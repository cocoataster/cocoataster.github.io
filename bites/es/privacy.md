---
layout: page
title: "Bites – Política de privacidad"
permalink: /bites/es/privacy/
lang: es
---
<p><a href="/bites/privacy/">EN</a> · <a href="/bites/es/privacy/">ES</a> · <a href="/bites/ca/privacy/">CA</a></p>

**Fecha de entrada en vigor:** octubre de 2026

Esta Política de privacidad explica cómo la app para iOS **Bites** («Bites», «la app») trata tu información. Bites es un diario personal de restaurantes y bares: tus listas «Visitados» y «Quiero ir», visitas, platos, valoraciones, notas, fotos y un mapa.

**En resumen:** Bites no tiene cuentas ni servidor propio. Tu diario se queda en tu dispositivo y, si la sincronización con iCloud está disponible y activada, en tu iCloud privado. El desarrollador no puede verlo. Bites no tiene publicidad, no te rastrea y no vende datos.

## 1. Responsable del tratamiento

Eric Sans
Barcelona, España
Web: https://cocoataster.com
Correo electrónico: privacy@cocoataster.com

## 2. Los datos de tu diario: guardados en tu dispositivo

Todo lo que introduces en Bites se guarda localmente en tu dispositivo con el framework SwiftData de Apple. Esto incluye:

- lugares (nombre, dirección, coordenadas, ciudad, tipo de cocina, nivel de precio, lista, etiquetas, notas, el enlace que pegaste y su imagen de vista previa)
- visitas (fecha, número de personas, valoración, notas)
- platos (nombre, precio, valoración)
- fotos

El desarrollador **no recibe, no almacena ni tiene acceso** a estos datos. No se necesita ninguna cuenta.

Tu diario también se incluye en las copias de seguridad habituales de tu dispositivo (copia en iCloud o en un ordenador), bajo tu control.

**Sincronización opcional con iCloud.** Si la sincronización con iCloud está disponible en tu versión de Bites y tienes la sesión de iCloud iniciada con iCloud activado para Bites, tu diario se sincroniza a través de tu **base de datos privada de CloudKit** en Apple. Solo tu Cuenta de Apple puede acceder a ella. El desarrollador no puede leerla. Puedes desactivarlo en cualquier momento en Ajustes de iOS › [tu nombre] › iCloud.

## 3. Información tratada al usar las funciones

### 3.1 Añadir un lugar desde un enlace de Google Maps

Cuando pegas un enlace de Google Maps, tu dispositivo usa el framework LinkPresentation de Apple para cargar ese enlace directamente desde los servidores de Google. Los enlaces admitidos son maps.app.goo.gl, goo.gl/maps, maps.google.* y google.com/maps.

La app lee de la página el nombre del lugar, la dirección, una imagen de vista previa y el enlace final, y los guarda en tu dispositivo.

Como tu dispositivo contacta con Google, Google recibe los datos técnicos habituales de una petición web, como tu dirección IP, el enlace solicitado y las cabeceras del dispositivo/navegador. Google los trata como responsable independiente según su propia política de privacidad (https://policies.google.com/privacy). Bites no usa una cuenta de Google, una clave de API de Google ni la API de Places de Google, y no envía nada más a Google.

Si pulsas «Abrir en Google Maps», el enlace guardado se abre en Google Maps o en tu navegador, donde se aplica la política de privacidad de Google.

### 3.2 Obtener coordenadas y mostrar el mapa (Apple Maps)

Cuando guardas un lugar o editas su dirección, la app envía **solo el texto de la dirección** al servicio de geocodificación de MapKit de Apple. Apple devuelve unas coordenadas y una ciudad, que se guardan en tu dispositivo.

El mapa usa Apple Maps (MapKit). Para mostrarlo, Apple recibe las peticiones necesarias para cargar el contenido del mapa. Apple trata estos datos según su propia política de privacidad (https://www.apple.com/es/legal/privacy/). El desarrollador no los recibe.

### 3.3 Tu ubicación (opcional)

Bites solo pide el permiso de ubicación «Cuando se use la app» **cuando eliges ordenar tus lugares por distancia**.

Tu ubicación se usa **únicamente en tu dispositivo**, para calcular distancias y mostrar tu posición en el mapa. No se guarda en tu diario ni se envía al desarrollador ni a las analíticas.

Si no lo permites, Bites ordena por los más recientes. Puedes cambiar este permiso en cualquier momento en Ajustes de iOS › Bites › Ubicación.

### 3.4 Fotos

Las fotos se añaden con el selector de fotos de iOS, que solo da a Bites las fotos que eliges. Bites no accede a toda tu fototeca y **no usa la cámara**.

Las fotos seleccionadas se reducen y se vuelven a codificar (máx. 1600 px). La copia guardada no conserva los metadatos del archivo original, como la ubicación GPS. Se guardan con tu diario como se describe en el apartado 2.

### 3.5 Analíticas de uso anónimas (TelemetryDeck)

Para entender qué funciones se usan y mejorar la app, Bites usa **TelemetryDeck**, un servicio de analíticas centrado en la privacidad. Bites envía unas pocas señales anónimas:

- se ha añadido un lugar
- se ha registrado una visita
- se ha mostrado la pantalla de Bites Pro
- se ha comprado Bites Pro

Cada señal incluye solo contexto técnico: cómo se originó (por ejemplo «enlace de Google Maps», «manual», «ajustes» o «temas»), el tipo de producto comprado y si es una versión de depuración/TestFlight. El SDK añade además información técnica estándar, como la versión de la app y de iOS, el tipo de dispositivo, el idioma/región y datos anónimos de sesión.

TelemetryDeck recibe un identificador anonimizado, no tu nombre, correo, Cuenta de Apple ni identificador publicitario. **Nunca se envía contenido del diario, fotos, nombres de lugares, direcciones ni tu ubicación.** Los datos no permiten identificarte ni rastrearte entre apps o webs.

Bites no usa el identificador publicitario de Apple (IDFA). No te rastrea según la definición de la Transparencia de Rastreo de Apps de Apple, por lo que no verás ninguna solicitud de rastreo.

Información de privacidad de TelemetryDeck: https://telemetrydeck.com/privacy/

### 3.6 Compras dentro de la app (Bites Pro)

Bites Pro se ofrece como suscripción mensual, suscripción anual o compra única de por vida. Los pagos, la facturación, los reembolsos y la gestión de suscripciones los gestiona íntegramente **Apple** a través del App Store, según sus condiciones y su política de privacidad.

El desarrollador nunca recibe tus datos de pago ni la identidad de tu Cuenta de Apple. En tu dispositivo, la app consulta a Apple qué compras están activas para desbloquear las funciones Pro. La app también lee información de transacciones del App Store para saber si es una versión de TestFlight/pruebas. El desarrollador solo ve informes de ventas agregados y anónimos de Apple.

### 3.7 Solicitud de valoración en el App Store

Después de registrar tu tercera visita, Bites puede pedir a Apple que muestre la solicitud estándar de valoración del App Store, como máximo una vez por versión de la app. Apple decide si la muestra y gestiona la valoración o reseña que envíes. La app solo guarda en tu dispositivo la versión en la que lo pidió por última vez.

### 3.8 Preferencias guardadas en tu dispositivo

Bites guarda localmente algunas preferencias, como el tema elegido. Nunca salen de tu dispositivo, salvo en tus propias copias de seguridad o sincronización.

## 4. Lo que Bites no hace

- No hay cuentas de usuario ni servidor del desarrollador.
- No hay publicidad ni SDK publicitarios.
- No se venden ni se alquilan datos personales.
- No hay rastreo entre apps o webs ni intermediarios de datos.
- No hay funciones sociales ni de amigos. Tu diario no se comparte con nadie.

## 5. Bases jurídicas (art. 6 RGPD)

- **Datos del diario en tu dispositivo y en tu iCloud privado:** el desarrollador no trata estos datos. Se guardan bajo tu control con los servicios de Apple.
- **Resolución de enlaces de Google Maps y geocodificación de direcciones:** ejecución del servicio que solicitas (art. 6.1.b). Son pasos necesarios para añadir el lugar que has pedido añadir.
- **Ubicación:** tu consentimiento (art. 6.1.a), dado mediante el permiso de iOS. Puedes retirarlo en cualquier momento en Ajustes de iOS.
- **Analíticas anónimas:** interés legítimo (art. 6.1.f) en entender el uso de las funciones y mejorar la app, con un método anonimizado y respetuoso con la privacidad que no se usa para rastrear.
- **Compras dentro de la app:** ejecución de un contrato (art. 6.1.b), con Apple como proveedor de pagos.
- **Solicitud de valoración:** interés legítimo (art. 6.1.f). Valorar es totalmente opcional.

## 6. Proveedores y terceros

| Proveedor | Función | Datos |
|---|---|---|
| Apple (Apple Distribution International Ltd., Irlanda / Apple Inc., EE. UU.) | App Store, compras dentro de la app, solicitud de valoración, mapas y geocodificación de MapKit, iCloud/CloudKit (si se usa), copias de seguridad | Según los apartados 2, 3.2, 3.6 y 3.7, conforme a la política de privacidad de Apple |
| Google (Google LLC / Google Ireland Ltd.) | Sirve el enlace de Google Maps que pegas | Datos técnicos de la petición (IP, enlace) al cargar el enlace (apartado 3.1) |
| TelemetryDeck | Analíticas de uso anónimas (encargado del tratamiento) | Señales anónimas descritas en el apartado 3.5 |

## 7. Transferencias internacionales

TelemetryDeck trata los datos de analíticas en la Unión Europea. Apple y Google pueden tratar datos fuera del Espacio Económico Europeo, incluidos los Estados Unidos.

Cuando lo hacen, se basan en garantías reconocidas por el RGPD, como el Marco de Privacidad de Datos UE-EE. UU. o las Cláusulas Contractuales Tipo de la Comisión Europea. Encontrarás los detalles en sus políticas de privacidad.

## 8. Conservación y supresión

- **Los datos del diario** permanecen en tu dispositivo, y en tu iCloud si se sincronizan, hasta que los borres.
  - Puedes borrar lugares, visitas, platos y fotos concretos desde la app. Al borrar un lugar se borran también sus visitas, platos y fotos.
  - Al eliminar la app se borran sus datos locales del dispositivo.
  - Los datos de iCloud se pueden gestionar o borrar en Ajustes de iOS › [tu nombre] › iCloud › Gestionar almacenamiento.
- **La ubicación** no la guarda Bites.
- **Las señales de analíticas** son anónimas. TelemetryDeck las conserva, principalmente de forma agregada, según su propia política de conservación. Como no pueden vincularse contigo, no se pueden recuperar ni suprimir para una persona concreta.
- **Los registros de compra** los conserva Apple según sus políticas.

## 9. Tus derechos

Según el RGPD y la Ley Orgánica 3/2018 (LOPDGDD), tienes estos derechos:

- acceso
- rectificación
- supresión
- limitación del tratamiento
- portabilidad
- oposición, incluida la oposición al tratamiento basado en el interés legítimo
- retirar tu consentimiento en cualquier momento, sin que afecte al tratamiento anterior

Como el desarrollador no conserva datos personales que te identifiquen, la mayoría de solicitudes se resuelven mejor directamente en tu dispositivo o con Apple o Google. Aun así, puedes escribir al desarrollador a privacy@cocoataster.com con cualquier duda o solicitud sobre privacidad.

También tienes derecho a presentar una reclamación ante una autoridad de control. En España es la **Agencia Española de Protección de Datos (AEPD)**, C/ Jorge Juan 6, 28001 Madrid, https://www.aepd.es.

## 10. Menores

Bites no está dirigida a menores. En España, los menores de 14 años solo deben usar apps que impliquen tratamiento de datos personales con el consentimiento de sus padres o tutores.

El desarrollador no recoge conscientemente datos personales de menores. Bites no recoge datos personales identificativos de nadie.

## 11. Seguridad

Tu diario está protegido por la seguridad de tu dispositivo y, si usas iCloud, por la seguridad de iCloud de Apple. Las peticiones de red de la app usan conexiones cifradas (HTTPS).

## 12. Cambios en esta política

Esta política puede actualizarse, por ejemplo al añadir nuevas funciones como la sincronización con iCloud. La versión actualizada se publicará con una nueva fecha de entrada en vigor. Los cambios importantes también se indicarán en las notas de la versión o en la app.

## 13. Contacto

Eric Sans, Barcelona, España
https://cocoataster.com
privacy@cocoataster.com

