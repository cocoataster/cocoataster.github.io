---
layout: post
title:  "Enhancing SwiftUI's TabView"
date:   2023-05-06 20:00:00 +0100
categories: jekyll update
---
SwiftUI gives us amazing out-of-the-box components to create the bare bones of our Apps, yet sometimes it fails to handle things we considered *"easy and simple"* in `UIKit`.

A few weeks ago I found a use case to update a screen's component given the user behavior with the `TabBar`. *"That should already be possible with the current tools"*, I thought to myself. Well, turns out it wasn't that straightforward.

I invite you to follow along my journey in this very special first post I've ever written :D

### Starting the Journey

The first attempt was to use our friend `.onTapGesture` on the `TabView`. Unfortunately (and not so shocking after thinking a bit about it) this overrides the built-in behavior, causing your Navigation to be completely broken.

{% highlight swift %}
TabView(selection: $selectedTab) { ... }
    .onTapGesture {
        // Congrats! You broke the App's Navigation.
    }
{% endhighlight %}

Then you start to think a bit more and believe there should be some existing modifier that can help you out. Like `.onChange`. But I'm sad to bring bad news again...

The problem with `.onChange` is that it will only trigger when the `newValue` is different from the `oldValue`. This helps if you wanna know when the user has changed from tab to tab, but it will **NOT** be useful to handle actions when the same tab is tapped.

And the same would happen if we were to use `.onReceive`. It will only provide a `value` when it's different from the old one.

{% highlight swift %}
TabView(selection: $selectedTab) { ... }
    .onChange(of: selectedTab) { newValue in
        // Triggers from one tab to another, but not tapping the same twice
    }

    .onReceive(Just(selectedTab)) { newValue in
        // Triggers from one tab to another, but not tapping the same twice
    }
{% endhighlight %}

So, is there any hope out there? Of course, there is! We just need a bit more rethinking.

### Thinking Deeper

What is it that we really want? What's the end goal of the changes we want to apply? Well, that would be to trigger an action when certain tab conditions are met. In our case, when a tab is tapped twice.

Let's set up our tabs first. For the sake of simplicity, we will have only 2:

{% highlight swift %}
enum Tab {
    case dashboard
    case settings
{% endhighlight %}

Now, let's write how the function comparing tabs would look like:

{% highlight swift %}
func onTabChange(old: Tab, new: Tab) -> Void {
    // Do some fancy logic here
}
{% endhighlight %}

When does this function need to be triggered? Every time a tab is tapped or, in other words, every time the `selectedTab` value is set.

For sure there should be something we can do within the `TabView` to fix this, right? Right?

### The TabView

If we take a look at `TabView`'s insides, we'll find there are 2 Generics used there:

* `SelectionValue`: which conforms to `Hashable`
    
* `Content`: which is the `View` to be renderer
    

{% highlight swift %}
struct TabView<SelectionValue, Content> where SelectionValue : Hashable, Content : View

init(
    selection: Binding<SelectionValue>?, 
    @ViewBuilder content: () -> Content
)
{% endhighlight %}

One key part we're missing is the `action` to be performed when tapping on the same tab again.

Let's fix that by creating an `extension` of `TabView`, and providing a handy `init` for our use case.

{% highlight swift %}
extension TabView {
    init(
        selection: Binding<SelectionValue>?,
        onTabChange: @escaping (_ old: SelectionValue, _ new: SelectionValue) -> Void,
        @ViewBuilder content: () -> Content
    ) {
        // Do something with onTabChange?
        self.init(
            selection: selection,
            content: content
        )
    }
}
{% endhighlight %}

We can now initialize a new `TabView` by providing the `onTabChange` action we created earlier since signatures match (kind of).

{% highlight swift %}
TabView(selection: $selectedTab, onTabChange: onTabChange) { ... }
{% endhighlight %}

Of course, `Tab` needs to conform `Hashable` because it's a requirement of `SelectionValue`.

{% highlight swift %}
extension Tab: Hashable { }
{% endhighlight %}

Now, wouldn't it be great if we could track `selection` changes? Not only the `newValue` but what's actually happening in there... so we can trigger an `action` whenever the new value is `set`. Let's take a closer look to the `Binding` struct.

### Binding

A `Binding<Value>` it's just a wrapper that holds data of type `Value`. So we can just create a new one using the default `init`.

{% highlight swift %}
Binding(get: () -> Value, set: (Value) -> Void)

// How implementation would look like

Binding(
    get: { wrappedValue },
    set: { newValue in
        wrappedValue = newValue
    }
)
{% endhighlight %}

**Aha**! There's just one thing missing. An `action` that will be triggered when the `newValue` is set.

Let's create an `extension` on `Binding` to make our lives easier. We need a function that takes an `action` with two input `Value` as an argument and returns a `Binding<Value>`.

{% highlight swift %}
extension Binding where Value: Hashable {
    func perform(_ action: @escaping (Value, Value) -> Void
    ) -> Binding<Value> {
        Binding(
            get: { wrappedValue },
            set: { newValue in
                action(wrappedValue, newValue)
                wrappedValue = newValue
            }
        )
    }
}
{% endhighlight %}

Great! Let's go back to our `TabView` extension and update our handy `init` so it makes use of this `perform` action.

{% highlight swift %}
extension TabView {
    init(
        selection: Binding<SelectionValue>?,
        onTabChange: @escaping (_ old: SelectionValue, _ new: SelectionValue) -> Void,
        @ViewBuilder content: () -> Content
    ) {
        self.init(
            selection: selection?.perform(onTabChange),
            content: content
        )
    }
}
{% endhighlight %}

Now we just need to use this new init in our `MainScreen.`

{% highlight swift %}
struct MainScreen: View {
    @State var selectedTab: Tab = .dashboard
    
    var body: some View {
        TabView(selection: $selectedTab, onTabChange: onTabChange) {
            Text("Dashboard Screen")
                .tabItem { Text("Dashboard")}
                .tag(Tab.dashboard)
            Text("Settings Screen")
                .tabItem { Text("Settings")}
                .tag(Tab.settings)
        }
    }

    func onTabChange(old: Tab, new: Tab) -> Void {
        print("From \(old) to \(new) tab")
    }
}
{% endhighlight %}

If your run the code, `onTabChange` will print every time you tab any tab, and provide both the old and new values.

### So, what's the use case?

Fair question my friend! The best-case scenario I can think of for this approach would be to `popToRoot` or just `popLast` presented screen when tapping the currently active tab.

And for that, I'm afraid you'll have to wait for the next post (since this is already too long, isn't it?).

Thank you for making it to the end!
