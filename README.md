# Learn-It (`v1.0`)

**Learn-It** is a 100% offline, local-only Android application built with Kotlin, Jetpack Compose, and Room SQLite for voice-first practice, memorization, and evaluation of:
- **99 Names of Allah (*Asma-ul-Husna*)** (`9×11` fixed recall map)
- **99 Names of Prophet Muhammad ﷺ (*Asma-un-Nabi*)** (`9×11` fixed recall map)
- **114 Surahs of the Holy Quran (*Asma-us-Suwar*)** (`6×19` fixed recall map)

---

## Key Features
- **Spontaneous Free-Recall Assessment (Speak & Write Modes):** Recite or type any Name/Surah in any order with real-time Arabic (`ar-SA`) and phonetic English transliteration matching, 3-second rolling phrase buffering, and a fixed-position circle recall map.
- **Master the Order (Sequential Levels, 50-Name Exam & Circular Puzzle Bonus):**
  - Orbiting target ring around the central microphone with `+10 pts` per independent recall in strict canonical order and `0 pts` for skips/hints.
  - 4 difficulty tiers (`Easy`, `Medium`, `Hard`, `V.Hard`), a `50-Name Exam`, and a `Puzzle Bonus Round` with circular `99 → 1` wrap-around.
  - Persistent SQLite Scoreboard and unlocked `L1, L2, L3...` progression.
- **Explore Directory & Quick View Gallery:** List, 2-Column Grid, and dense `Quick View` micro-grid with spring zoom-in lightbox and bundled offline pronunciation audio (`312` MP3 clips compiled inside the APK).
- **50-Hadith Offline Reader:** Distraction-free horizontal reader with 50 authentic narrations and native WhatsApp sharing.
- **Progress & Analytics Dashboard:** Spaced-review mastery tracking, chronological session history, and comparative recall insights.

---

## Installing the Android APK (`v1.0`)
1. Download the `v1.0` APK (`app-debug.apk`) from the **GitHub Releases** page.
2. On your Android device, open **Settings → Security** (or **Apps → Special app access → Install unknown apps**) and enable **Install from Unknown Sources** for your browser or file manager.
3. Tap the downloaded `.apk` file and follow the on-screen prompt to install **Learn-It**.

---

## Repository Structure
```text
learn-it/
├── app/
│   ├── build.gradle.kts          # Android app module & v1.0 version config
│   └── src/
│       ├── main/
│       │   ├── AndroidManifest.xml
│       │   ├── assets/           # Offline JSON datasets & 312 bundled MP3s
│       │   ├── java/com/example/ # Kotlin + Jetpack Compose + Room SQLite source
│       │   └── res/              # Fonts, drawables, strings, and themes
│       └── test/                 # Unit & Robolectric tests
├── gradle/                       # Gradle wrapper & version catalog
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

---

## Building Locally
1. Open the project in **Android Studio** (or use `./gradlew assembleDebug` with `ANDROID_HOME` configured).
2. Ensure JDK 11+ and Android SDK 36 are installed.
3. Run `./gradlew assembleDebug` to build the APK.
