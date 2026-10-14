---
layout: page
title: "Bites – Privacy Policy"
permalink: /bites/privacy/
---
<p><a href="/bites/privacy/">EN</a> · <a href="/bites/es/privacy/">ES</a> · <a href="/bites/ca/privacy/">CA</a></p>

**Effective date:** October 2026

This Privacy Policy explains how the iOS app **Bites** ("Bites", "the app") handles your information. Bites is a personal diary of restaurants and bars: your "Been" and "Want to go" lists, visits, dishes, ratings, notes, photos and a map.

**The short version:** Bites has no accounts and no developer server. Your diary stays on your device, and in your own private iCloud if iCloud sync is available and turned on. The developer cannot see it. Bites has no ads, does not track you and does not sell data.

## 1. Who is responsible (data controller)

Eric Sans
Barcelona, Spain
Website: https://cocoataster.com
Email: [CONTACT EMAIL]

## 2. Your diary data: stored on your device

Everything you enter in Bites is stored locally on your device using Apple's SwiftData framework. This includes:

- places (name, address, coordinates, city, cuisine, price level, list, tags, notes, the link you pasted and its preview image)
- visits (date, number of people, rating, notes)
- dishes (name, price, rating)
- photos

The developer **does not receive, store or have access to** this data. No account is required.

Your diary is also included in your normal device backups (iCloud Backup or a computer backup), under your own control.

**Optional iCloud sync.** If iCloud sync is available in your version of Bites and you are signed in to iCloud with iCloud enabled for Bites, your diary is synced through your **private CloudKit database** at Apple. Only your Apple Account can access that database. The developer cannot read it. You can turn this off at any time in iOS Settings › [your name] › iCloud.

## 3. Information processed when you use features

### 3.1 Adding a place from a Google Maps link

When you paste a Google Maps link, your device uses Apple's LinkPresentation framework to load that link directly from Google's servers. Supported links are maps.app.goo.gl, goo.gl/maps, maps.google.* and google.com/maps.

The app reads the place name, the address, a preview image and the final link from the page, and stores them on your device.

Because your device contacts Google, Google receives the usual technical data of a web request, such as your IP address, the requested link and device/browser headers. Google processes this as an independent controller under its own privacy policy (https://policies.google.com/privacy). Bites does not use a Google account, a Google API key or Google's Places API, and sends nothing else to Google.

When you tap "Open in Google Maps", the saved link opens in Google Maps or your browser, where Google's privacy policy applies.

### 3.2 Finding coordinates and showing the map (Apple Maps)

When you save a place or edit its address, the app sends **only the address text** to Apple's MapKit geocoding service. Apple returns coordinates and a city, which are stored on your device.

The map uses Apple Maps (MapKit). To display it, Apple receives the requests needed to load map content. Apple processes this data under its own privacy policy (https://www.apple.com/legal/privacy/). The developer does not receive it.

### 3.3 Your location (optional)

Bites asks for "While Using the App" location permission **only when you choose to sort your places by distance**.

Your location is used **on your device only**, to calculate distances and to show your position on the map. It is not stored in your diary and is not sent to the developer or to analytics.

If you decline, Bites sorts by most recent instead. You can change this permission at any time in iOS Settings › Bites › Location.

### 3.4 Photos

You add photos with the iOS photo picker, which only gives Bites the photos you select. Bites does not get access to your whole library and **does not use the camera**.

Selected photos are downscaled and re-encoded (max. 1600 px). The stored copy does not keep the original file's metadata, such as GPS location. Photos are stored with your diary as described in section 2.

### 3.5 Anonymous usage analytics (TelemetryDeck)

To understand which features are used and improve the app, Bites uses **TelemetryDeck**, a privacy-focused analytics service. Bites sends a few anonymous signals:

- a place was added
- a visit was logged
- the Bites Pro screen was shown
- Bites Pro was purchased

Each signal includes only technical context: how it was triggered (for example "Google Maps link", "manual", "settings" or "themes"), the purchased product type, and whether the build is a debug/TestFlight build. The SDK also adds standard technical information, such as app and iOS version, device type, language/region and anonymous session data.

TelemetryDeck receives an anonymised identifier, not your name, email, Apple Account or advertising identifier. **No diary content, photos, place names, addresses or location** is ever sent. The data cannot be used to identify you or to track you across apps or websites.

Bites does not use Apple's advertising identifier (IDFA). It does not track you as defined by Apple's App Tracking Transparency, so you will not see a tracking prompt.

TelemetryDeck's privacy information: https://telemetrydeck.com/privacy/

### 3.6 In-app purchases (Bites Pro)

Bites Pro is offered as a monthly subscription, an annual subscription or a one-time lifetime purchase. Payments, billing, refunds and subscription management are handled entirely by **Apple** through the App Store, under Apple's terms and privacy policy.

The developer never receives your payment details or Apple Account identity. On your device, the app checks with Apple which purchases are active, to unlock Pro features. The app also reads App Store transaction information to tell whether it is a TestFlight/test build. The developer only sees aggregated, anonymous sales reports from Apple.

### 3.7 App Store rating prompt

After you log your third visit, Bites may ask Apple to show the standard App Store rating prompt, at most once per app version. Apple decides whether to show it and handles any rating or review you submit. The app only stores, on your device, the app version in which it last asked.

### 3.8 Settings stored on your device

Bites stores a few preferences locally, such as your chosen theme. These never leave your device except as part of your own backups or sync.

## 4. What Bites does not do

- No user accounts and no developer server.
- No advertising and no advertising SDKs.
- No sale or rental of personal data.
- No tracking across apps or websites, and no data brokers.
- No social or friends features. Your diary is not shared with anyone.

## 5. Legal bases (GDPR Art. 6)

- **Diary data on your device and in your private iCloud:** the developer does not process this data. It is stored under your own control with Apple's services.
- **Resolving Google Maps links and geocoding addresses:** performance of the service you request (Art. 6(1)(b)). These steps are needed to add the place you asked to add.
- **Location:** your consent (Art. 6(1)(a)), given through the iOS permission. You can withdraw it at any time in iOS Settings.
- **Anonymous analytics:** legitimate interest (Art. 6(1)(f)) in understanding feature usage and improving the app, using a privacy-friendly, anonymised method that is not used for tracking.
- **In-app purchases:** performance of a contract (Art. 6(1)(b)), with Apple as the payment provider.
- **Rating prompt:** legitimate interest (Art. 6(1)(f)). Rating is entirely optional.

## 6. Service providers and third parties

| Provider | Role | Data |
|---|---|---|
| Apple (Apple Distribution International Ltd., Ireland / Apple Inc., USA) | App Store, in-app purchases, rating prompt, MapKit maps and geocoding, iCloud/CloudKit (if used), device backups | As described in sections 2, 3.2, 3.6 and 3.7, under Apple's privacy policy |
| Google (Google LLC / Google Ireland Ltd.) | Serves the Google Maps link you paste | Technical request data (IP address, link) when the link is loaded (section 3.1) |
| TelemetryDeck | Anonymous usage analytics (processor) | Anonymous signals described in section 3.5 |

## 7. International transfers

TelemetryDeck processes analytics data in the European Union. Apple and Google may process data outside the European Economic Area, including in the United States.

Where they do, they rely on safeguards recognised under the GDPR, such as the EU–US Data Privacy Framework or the European Commission's Standard Contractual Clauses. Details are in their privacy policies.

## 8. Retention and deletion

- **Diary data** stays on your device, and in your iCloud if synced, until you delete it.
  - You can delete individual places, visits, dishes and photos in the app. Deleting a place also deletes its visits, dishes and photos.
  - Deleting the app removes its local data from the device.
  - iCloud data can be managed or deleted in iOS Settings › [your name] › iCloud › Manage Storage.
- **Location** is not stored by Bites.
- **Analytics** signals are anonymous. TelemetryDeck retains them, mostly in aggregated form, under its own retention policy. Because they cannot be linked to you, they cannot be retrieved or deleted for a specific person.
- **Purchase records** are kept by Apple under Apple's policies.

## 9. Your rights

Under the GDPR and the Spanish data protection law (LOPDGDD), you have these rights:

- access
- rectification
- erasure
- restriction of processing
- data portability
- objection, including to processing based on legitimate interest
- withdrawing consent at any time, without affecting earlier processing

Because the developer holds no personal data that identifies you, most requests are best handled directly on your device or with Apple or Google. You can still contact the developer at [CONTACT EMAIL] with any privacy question or request.

You also have the right to lodge a complaint with a supervisory authority. In Spain this is the **Agencia Española de Protección de Datos (AEPD)**, C/ Jorge Juan 6, 28001 Madrid, https://www.aepd.es.

## 10. Children

Bites is not directed at children. In Spain, people under 14 should use apps that involve processing of personal data only with the consent of a parent or guardian.

The developer does not knowingly collect personal data from children. Bites does not collect identifying personal data from anyone.

## 11. Security

Your diary is protected by your device's security and, if you use iCloud, by Apple's iCloud security. Network requests made by the app use encrypted connections (HTTPS).

## 12. Changes to this policy

This policy may be updated, for example when new features such as iCloud sync are added. The updated version will be published with a new effective date. Significant changes will also be noted in the app's release notes or in the app.

## 13. Contact

Eric Sans, Barcelona, Spain
https://cocoataster.com
[CONTACT EMAIL]

