# Cristian Ramón Noguera

Desarrollador de software · iOS, Android y backend · Granada

Ingeniero informático por la Universidad de Granada (2022 – 2026, mención en Computación y Sistemas Inteligentes). Desde enero de 2026 desarrollo en [GeoNotary](https://geonotary.com), una empresa de peritaje informático y certificación de evidencia digital, donde llevo las apps móviles, el backend y el servidor de producción.

El código de estos proyectos es propiedad de la empresa y está en repositorios privados. Aquí resumo qué hace cada producto y qué he hecho yo en él.

[Portfolio web](https://dunkurunku.github.io) · [Currículum en PDF](https://dunkurunku.github.io/assets/Curriculum-Cristian-Ramon-Noguera.pdf) · xxcristianxx2004@gmail.com

---

## GeoNotary

**Certifica la ubicación del usuario con validez judicial.** Registra la posición con sellado temporal y resumen criptográfico, y construye un modelo de identidad a partir de los patrones de movimiento para acreditar que el registro es del propio usuario. Se usa en defensa legal y en acreditación de residencia fiscal.

[App Store](https://apps.apple.com/es/app/geonotary/id6742685214) · [Google Play](https://play.google.com/store/apps/details?id=com.geonotary.app)

**Mi trabajo**
- Cliente Android desde cero hasta su publicación en Google Play: Kotlin, Jetpack Compose, Room y Retrofit, con paridad funcional con la app iOS (login federado, sincronización, suscripciones, informe de fallos, internacionalización).
- Rechazo de ubicaciones simuladas y verificación de integridad de la instalación con Play Integrity.
- En la app iOS (Swift, SwiftUI, Core Data, Core Location): corrección de la pérdida de días completos de registro y de los cierres del sistema por memoria en segundo plano, procesando el histórico por ventanas acotadas.
- Corrección de una fuga de datos entre entrenamiento y validación en el modelo de identidad, que daba métricas optimistas.

## WhatsPericialApp

**Certificación de conversaciones de WhatsApp como prueba pericial.** Adquisición asistida de la conversación, integridad de la evidencia y generación del informe pericial. Publicada en iOS y Android.

[App Store](https://apps.apple.com/es/app/whatspericialapp/id6772326675) · [Google Play](https://play.google.com/store/apps/details?id=com.whatspericial.app)

**Mi trabajo**
- Port completo de la app iOS a Android (49 ficheros Kotlin), incluida la sesión asistida con LiveKit y Play Integrity.
- Backend PHP y Node.js: fallos de escala con conversaciones grandes (inserción por lotes, sustitución del motor de generación de PDF), integridad SHA-256 de la evidencia y cadena de custodia.
- Auditoría de seguridad: endpoints sin autenticación, verificación de firma del webhook de Stripe, credenciales fuera del código, registro de tráfico HTTP eliminado en compilaciones de distribución.
- Sitio web en React, Vite y Tailwind, y despliegues en el servidor de producción.

## Museo interactivo con Leap Motion · código abierto

Museo temático de Minecraft en el que el visitante interactúa sin tocar nada: tótems web manejados con las manos mediante un sensor Leap Motion y three.js, y una app Android complementaria con escáner QR, inventario y logros. Proyecto de la asignatura Nuevos Paradigmas de Interacción (UGR).

[Código y vídeo](https://github.com/dunkurunku/museo-minecraft)

## Predicción de biomasa desde una foto · Kaggle · código abierto

Competición CSIRO – Image2Biomass en Kaggle: estimar la biomasa de un pasto a partir de una única imagen cenital, separando la materia viva de la muerta, con solo 357 fotos de entrenamiento. Comparamos cuatro estrategias (DINOv2 con cabezas de regresión, destilación con información privilegiada, ensemble ConvNeXt + EfficientNet y descriptores clásicos) y escribimos la memoria como un artículo científico. Hallazgo clave: validar por fechas destapa una fuga de datos que inflaba el R² de 0,75 a 0,81. Proyecto en grupo para la competición, pensado para poner a prueba nuestros conocimientos y habilidades de Deep Learning sobre un problema real.

[Código y memoria](https://github.com/dunkurunku/image2biomass-kaggle)

## Compilador con Flex y Bison · código abierto

Compilador completo en C para un pequeño lenguaje imperativo: léxico, sintáctico LALR(1), semántico con tabla de símbolos y ámbitos, cuádruplos y generación de C. Con pruebas automáticas y GitHub Actions. Proyecto individual de Procesadores de Lenguajes (UGR).

[Código](https://github.com/dunkurunku/compilador-flex-bison)

---

## Tecnologías

| | |
|---|---|
| **Lenguajes** | Swift, Kotlin, C++, C, Java, C#, Python, PHP, JavaScript, SQL, Bash, R, Prolog, CLIPS |
| **iOS** | SwiftUI, Core Data, Core Location, Core Motion, tareas en segundo plano, App Attest, Xcode, App Store Connect, TestFlight |
| **Android** | Jetpack Compose, Room, Retrofit, Play Integrity, Play Billing, Android Studio, Google Play Console |
| **Backend** | PHP, Node.js, MySQL, APIs REST, Socket.IO, LiveKit, Stripe y webhooks, Firebase (Analytics, Crashlytics, FCM) |
| **Sistemas** | Linux, Nginx, TLS, cron, rsync, despliegue y rollback, Git y GitHub |
| **Web** | React, Vite, Tailwind, HTML y CSS |
| **Datos e IA** | Análisis de datos en Python, aprendizaje automático, MPI y concurrencia, desarrollo asistido con IA (Claude Code, MCP) |
| **Seguridad** | Auditoría de backend, integridad SHA-256, cadena de custodia, RGPD |

## Formación

**Grado en Ingeniería Informática** · Universidad de Granada · 2022 – 2026
Mención en Computación y Sistemas Inteligentes. Prácticas de empresa (12 ECTS) en GeoNotary S.L.

Español nativo · Inglés B2
