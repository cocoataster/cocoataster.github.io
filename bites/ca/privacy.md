---
layout: page
title: "Bites – Política de privacitat"
permalink: /bites/ca/privacy/
lang: ca
---
<p><a href="/bites/privacy/">EN</a> · <a href="/bites/es/privacy/">ES</a> · <a href="/bites/ca/privacy/">CA</a></p>

**Data d'entrada en vigor:** octubre de 2026

Aquesta Política de privadesa explica com l'app per a iOS **Bites** («Bites», «l'app») tracta la teva informació. Bites és un diari personal de restaurants i bars: les teves llistes «Visitats» i «Vull anar-hi», visites, plats, valoracions, notes, fotos i un mapa.

**En resum:** Bites no té comptes ni servidor propi. El teu diari es queda al teu dispositiu i, si la sincronització amb iCloud està disponible i activada, al teu iCloud privat. El desenvolupador no el pot veure. Bites no té publicitat, no et fa seguiment i no ven dades.

## 1. Responsable del tractament

Eric Sans
Barcelona, Espanya
Web: https://cocoataster.com
Correu electrònic: [CONTACT EMAIL]

## 2. Les dades del teu diari: desades al teu dispositiu

Tot el que introdueixes a Bites es desa localment al teu dispositiu amb el framework SwiftData d'Apple. Això inclou:

- llocs (nom, adreça, coordenades, ciutat, tipus de cuina, nivell de preu, llista, etiquetes, notes, l'enllaç que vas enganxar i la seva imatge de previsualització)
- visites (data, nombre de persones, valoració, notes)
- plats (nom, preu, valoració)
- fotos

El desenvolupador **no rep, no emmagatzema ni té accés** a aquestes dades. No cal cap compte.

El teu diari també s'inclou a les còpies de seguretat habituals del dispositiu (còpia a iCloud o en un ordinador), sota el teu control.

**Sincronització opcional amb iCloud.** Si la sincronització amb iCloud està disponible a la teva versió de Bites i tens la sessió d'iCloud iniciada amb iCloud activat per a Bites, el teu diari se sincronitza a través de la teva **base de dades privada de CloudKit** a Apple. Només el teu Compte d'Apple hi pot accedir. El desenvolupador no la pot llegir. Ho pots desactivar en qualsevol moment a Configuració d'iOS › [el teu nom] › iCloud.

## 3. Informació tractada en fer servir les funcions

### 3.1 Afegir un lloc des d'un enllaç de Google Maps

Quan enganxes un enllaç de Google Maps, el teu dispositiu fa servir el framework LinkPresentation d'Apple per carregar aquest enllaç directament des dels servidors de Google. Els enllaços admesos són maps.app.goo.gl, goo.gl/maps, maps.google.* i google.com/maps.

L'app llegeix de la pàgina el nom del lloc, l'adreça, una imatge de previsualització i l'enllaç final, i els desa al teu dispositiu.

Com que el teu dispositiu contacta amb Google, Google rep les dades tècniques habituals d'una petició web, com ara la teva adreça IP, l'enllaç sol·licitat i les capçaleres del dispositiu/navegador. Google les tracta com a responsable independent segons la seva pròpia política de privadesa (https://policies.google.com/privacy). Bites no fa servir cap compte de Google, cap clau d'API de Google ni l'API de Places de Google, i no envia res més a Google.

Si toques «Obrir a Google Maps», l'enllaç desat s'obre a Google Maps o al navegador, on s'aplica la política de privadesa de Google.

### 3.2 Obtenir coordenades i mostrar el mapa (Apple Maps)

Quan deses un lloc o n'edites l'adreça, l'app envia **només el text de l'adreça** al servei de geocodificació de MapKit d'Apple. Apple retorna unes coordenades i una ciutat, que es desen al teu dispositiu.

El mapa fa servir Apple Maps (MapKit). Per mostrar-lo, Apple rep les peticions necessàries per carregar el contingut del mapa. Apple tracta aquestes dades segons la seva pròpia política de privadesa (https://www.apple.com/legal/privacy/). El desenvolupador no les rep.

### 3.3 La teva ubicació (opcional)

Bites només demana el permís d'ubicació «Mentre s'utilitza l'app» **quan tries ordenar els teus llocs per distància**.

La teva ubicació es fa servir **només al teu dispositiu**, per calcular distàncies i mostrar la teva posició al mapa. No es desa al teu diari ni s'envia al desenvolupador ni a les analítiques.

Si no ho permets, Bites ordena pels més recents. Pots canviar aquest permís en qualsevol moment a Configuració d'iOS › Bites › Ubicació.

### 3.4 Fotos

Les fotos s'afegeixen amb el selector de fotos d'iOS, que només dona a Bites les fotos que tries. Bites no accedeix a tota la fototeca i **no fa servir la càmera**.

Les fotos seleccionades es redueixen i es tornen a codificar (màx. 1600 px). La còpia desada no conserva les metadades del fitxer original, com ara la ubicació GPS. Es desen amb el teu diari tal com es descriu a l'apartat 2.

### 3.5 Analítiques d'ús anònimes (TelemetryDeck)

Per entendre quines funcions es fan servir i millorar l'app, Bites utilitza **TelemetryDeck**, un servei d'analítiques centrat en la privadesa. Bites envia unes poques senyals anònimes:

- s'ha afegit un lloc
- s'ha registrat una visita
- s'ha mostrat la pantalla de Bites Pro
- s'ha comprat Bites Pro

Cada senyal inclou només context tècnic: com s'ha originat (per exemple «enllaç de Google Maps», «manual», «configuració» o «temes»), el tipus de producte comprat i si és una versió de depuració/TestFlight. L'SDK hi afegeix informació tècnica estàndard, com ara la versió de l'app i d'iOS, el tipus de dispositiu, l'idioma/regió i dades anònimes de sessió.

TelemetryDeck rep un identificador anonimitzat, no el teu nom, correu, Compte d'Apple ni identificador publicitari. **Mai no s'envia contingut del diari, fotos, noms de llocs, adreces ni la teva ubicació.** Les dades no permeten identificar-te ni fer-te seguiment entre apps o webs.

Bites no fa servir l'identificador publicitari d'Apple (IDFA). No et fa seguiment segons la definició de la Transparència del Seguiment d'Apps d'Apple, de manera que no veuràs cap sol·licitud de seguiment.

Informació de privadesa de TelemetryDeck: https://telemetrydeck.com/privacy/

### 3.6 Compres dins de l'app (Bites Pro)

Bites Pro s'ofereix com a subscripció mensual, subscripció anual o compra única per a sempre. Els pagaments, la facturació, els reemborsaments i la gestió de subscripcions els gestiona íntegrament **Apple** a través de l'App Store, segons les seves condicions i la seva política de privadesa.

El desenvolupador mai no rep les teves dades de pagament ni la identitat del teu Compte d'Apple. Al teu dispositiu, l'app consulta a Apple quines compres estan actives per desbloquejar les funcions Pro. L'app també llegeix informació de transaccions de l'App Store per saber si és una versió de TestFlight/proves. El desenvolupador només veu informes de vendes agregats i anònims d'Apple.

### 3.7 Sol·licitud de valoració a l'App Store

Després de registrar la teva tercera visita, Bites pot demanar a Apple que mostri la sol·licitud estàndard de valoració de l'App Store, com a màxim un cop per versió de l'app. Apple decideix si la mostra i gestiona la valoració o ressenya que enviïs. L'app només desa al teu dispositiu la versió en què ho va demanar per última vegada.

### 3.8 Preferències desades al teu dispositiu

Bites desa localment algunes preferències, com el tema escollit. Mai no surten del teu dispositiu, excepte a les teves pròpies còpies de seguretat o sincronització.

## 4. El que Bites no fa

- No hi ha comptes d'usuari ni servidor del desenvolupador.
- No hi ha publicitat ni SDK publicitaris.
- No es venen ni es lloguen dades personals.
- No hi ha seguiment entre apps o webs ni intermediaris de dades.
- No hi ha funcions socials ni d'amics. El teu diari no es comparteix amb ningú.

## 5. Bases jurídiques (art. 6 RGPD)

- **Dades del diari al teu dispositiu i al teu iCloud privat:** el desenvolupador no tracta aquestes dades. Es desen sota el teu control amb els serveis d'Apple.
- **Resolució d'enllaços de Google Maps i geocodificació d'adreces:** execució del servei que sol·licites (art. 6.1.b). Són passos necessaris per afegir el lloc que has demanat afegir.
- **Ubicació:** el teu consentiment (art. 6.1.a), donat mitjançant el permís d'iOS. El pots retirar en qualsevol moment a Configuració d'iOS.
- **Analítiques anònimes:** interès legítim (art. 6.1.f) a entendre l'ús de les funcions i millorar l'app, amb un mètode anonimitzat i respectuós amb la privadesa que no es fa servir per fer seguiment.
- **Compres dins de l'app:** execució d'un contracte (art. 6.1.b), amb Apple com a proveïdor de pagaments.
- **Sol·licitud de valoració:** interès legítim (art. 6.1.f). Valorar és totalment opcional.

## 6. Proveïdors i tercers

| Proveïdor | Funció | Dades |
|---|---|---|
| Apple (Apple Distribution International Ltd., Irlanda / Apple Inc., EUA) | App Store, compres dins de l'app, sol·licitud de valoració, mapes i geocodificació de MapKit, iCloud/CloudKit (si s'utilitza), còpies de seguretat | Segons els apartats 2, 3.2, 3.6 i 3.7, d'acord amb la política de privadesa d'Apple |
| Google (Google LLC / Google Ireland Ltd.) | Serveix l'enllaç de Google Maps que enganxes | Dades tècniques de la petició (IP, enllaç) en carregar l'enllaç (apartat 3.1) |
| TelemetryDeck | Analítiques d'ús anònimes (encarregat del tractament) | Senyals anònimes descrites a l'apartat 3.5 |

## 7. Transferències internacionals

TelemetryDeck tracta les dades d'analítiques a la Unió Europea. Apple i Google poden tractar dades fora de l'Espai Econòmic Europeu, inclosos els Estats Units.

Quan ho fan, es basen en garanties reconegudes pel RGPD, com el Marc de Privadesa de Dades UE-EUA o les Clàusules Contractuals Tipus de la Comissió Europea. En trobaràs els detalls a les seves polítiques de privadesa.

## 8. Conservació i supressió

- **Les dades del diari** romanen al teu dispositiu, i al teu iCloud si se sincronitzen, fins que les esborris.
  - Pots esborrar llocs, visites, plats i fotos concrets des de l'app. En esborrar un lloc també s'esborren les seves visites, plats i fotos.
  - En eliminar l'app s'esborren les seves dades locals del dispositiu.
  - Les dades d'iCloud es poden gestionar o esborrar a Configuració d'iOS › [el teu nom] › iCloud › Gestionar l'emmagatzematge.
- **La ubicació** no la desa Bites.
- **Les senyals d'analítiques** són anònimes. TelemetryDeck les conserva, principalment de forma agregada, segons la seva pròpia política de conservació. Com que no es poden vincular amb tu, no es poden recuperar ni suprimir per a una persona concreta.
- **Els registres de compra** els conserva Apple segons les seves polítiques.

## 9. Els teus drets

D'acord amb el RGPD i la Llei orgànica 3/2018 (LOPDGDD), tens aquests drets:

- accés
- rectificació
- supressió
- limitació del tractament
- portabilitat
- oposició, inclosa l'oposició al tractament basat en l'interès legítim
- retirar el teu consentiment en qualsevol moment, sense que afecti el tractament anterior

Com que el desenvolupador no conserva dades personals que t'identifiquin, la majoria de sol·licituds es resolen millor directament al teu dispositiu o amb Apple o Google. Tot i així, pots escriure al desenvolupador a [CONTACT EMAIL] amb qualsevol dubte o sol·licitud sobre privadesa.

També tens dret a presentar una reclamació davant d'una autoritat de control. A Espanya és l'**Agencia Española de Protección de Datos (AEPD)**, C/ Jorge Juan 6, 28001 Madrid, https://www.aepd.es.

## 10. Menors

Bites no està adreçada a menors. A Espanya, els menors de 14 anys només han de fer servir apps que impliquin tractament de dades personals amb el consentiment dels pares o tutors.

El desenvolupador no recull conscientment dades personals de menors. Bites no recull dades personals identificatives de ningú.

## 11. Seguretat

El teu diari està protegit per la seguretat del teu dispositiu i, si fas servir iCloud, per la seguretat d'iCloud d'Apple. Les peticions de xarxa de l'app fan servir connexions xifrades (HTTPS).

## 12. Canvis en aquesta política

Aquesta política es pot actualitzar, per exemple en afegir noves funcions com la sincronització amb iCloud. La versió actualitzada es publicarà amb una nova data d'entrada en vigor. Els canvis importants també s'indicaran a les notes de la versió o a l'app.

## 13. Contacte

Eric Sans, Barcelona, Espanya
https://cocoataster.com
[CONTACT EMAIL]

