# Cristian Ramón Noguera

Software, AI & Mobile Developer · iOS, Android, backend and AI · Granada, Spain

Computer Engineer from the University of Granada (2022 – 2026, specialisation in Computing and Intelligent Systems). Since December 2025 I've been working at [GeoNotary](https://geonotary.com), a digital forensics and evidence certification company, where I work on the mobile apps, the backend, the production server and AI features trained on real data.

The code of the company products lives in private repositories, so below I summarise what each product does and which parts I built. The rest are public repositories.

[Portfolio](https://dunkurunku.github.io) · [Resume (PDF)](https://dunkurunku.github.io/assets/Resume-Cristian-Ramon-Noguera.pdf) · [LinkedIn](https://www.linkedin.com/in/cristian-ramon-noguera) · crisrn04@icloud.com

---

## GeoNotary

**Certifies the user's location with legal validity.** It records the position with a timestamp and a cryptographic digest, and builds an identity model from movement patterns to show that the record belongs to the user. Used in legal defence and to prove tax residency.

[App Store](https://apps.apple.com/es/app/geonotary/id6742685214) · [Google Play](https://play.google.com/store/apps/details?id=com.geonotary.app)

**What I did**
- Android client from scratch through to its release on Google Play: Kotlin, Jetpack Compose, Room and Retrofit, with feature parity with the iOS app (federated login, sync, subscriptions, crash reporting, localisation).
- Rejection of mocked locations and install integrity checks with Play Integrity.
- On iOS (Swift, SwiftUI, Core Data, Core Location): fixed the loss of whole days of records and out-of-memory kills in the background by processing history in bounded windows.
- Developed an AI model trained on real usage data, and fixed a data leak between training and validation in the identity model that was producing optimistic metrics.

## WhatsPericialApp

**Certifies WhatsApp conversations as forensic evidence.** Assisted acquisition of the conversation, evidence integrity and generation of the expert report. Released on iOS and Android.

[App Store](https://apps.apple.com/es/app/whatspericialapp/id6772326675) · [Google Play](https://play.google.com/store/apps/details?id=com.whatspericial.app)

**What I did**
- Full port of the iOS app to Android (49 Kotlin files), including the real-time assisted session with LiveKit and Play Integrity.
- Worked on the real-time voice AI agent in Python (LiveKit, OpenAI API) that guides users through the session.
- PHP and Node.js backend: scaling issues with large conversations (batch inserts, replacing the PDF engine), SHA-256 evidence integrity and chain of custody.
- Security audit: unauthenticated endpoints, Stripe webhook signature verification, credentials moved out of the code, HTTP traffic logging removed from release builds.
- Company website in React, Vite and Tailwind, and deployments on the production server.

## Evidence Vault API · open source

REST API to keep files as evidence: every file is registered with its SHA-256 digest and a timestamp, and every action is appended to a hash-chained chain of custody that detects tampering. Python, FastAPI, SQLAlchemy, PostgreSQL, JWT authentication, document summaries with the Claude API, automated tests, Docker and GitHub Actions.

[Code](https://github.com/dunkurunku/evidence-vault-api)

## Pasture biomass from a single photo · Kaggle · open source

CSIRO – Image2Biomass competition on Kaggle: estimate pasture biomass from a single top-down image, separating live from dead matter, with only 357 training photos. We compared four strategies (DINOv2 with regression heads, distillation with privileged information, a ConvNeXt + EfficientNet ensemble and classical descriptors), detected and fixed data leakage in validation, and wrote the report as a scientific paper. Team project for the competition.

[Code and report](https://github.com/dunkurunku/image2biomass-kaggle)

## Interactive museum with Leap Motion · open source

A Minecraft-themed museum where visitors interact without touching anything: web kiosks controlled by hand through a Leap Motion sensor and three.js, plus a companion Android app with a QR scanner, inventory and achievements. A natural interaction project with gesture sensors.

[Code and video](https://github.com/dunkurunku/museo-minecraft)

## Compiler with Flex and Bison · open source

A complete compiler in C for a small imperative language: lexer, LALR(1) parser, semantic analysis with a symbol table and scopes, quadruples and C generation. With automated tests and GitHub Actions. Individual project.

[Code](https://github.com/dunkurunku/compilador-flex-bison)

---

## Tech stack

| | |
|---|---|
| **Languages** | Swift, Kotlin, Python, PHP, JavaScript, Java, C/C++, SQL, Bash |
| **iOS** | SwiftUI, Core Data, Core Location, Core Motion, background tasks, App Attest, Xcode, App Store Connect, TestFlight |
| **Android** | Jetpack Compose, Room, Retrofit, Play Integrity, Play Billing, Android Studio, Google Play Console |
| **Backend** | PHP, Node.js, FastAPI, REST APIs, Socket.IO, LiveKit, Stripe and webhooks, Firebase (Analytics, Crashlytics, FCM) |
| **Data** | PostgreSQL, MySQL, MongoDB |
| **Systems** | Linux, Nginx, TLS, cron, Docker, Google Cloud, deployments and rollbacks, Git and GitHub Actions |
| **Web** | React, Vite, Tailwind, HTML and CSS |
| **AI and data** | LLMs and voice agents (OpenAI API, Claude API), scikit-learn, fastai, PyTorch, CNNs, data mining and analysis in Python |

## Education

**Bachelor's degree in Computer Engineering** · University of Granada · 2022 – 2026
Specialisation in Computing and Intelligent Systems. Internship at GeoNotary S.L.

Spanish (native) · English (B2)
