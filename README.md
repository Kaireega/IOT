# IOT

Android home automation app for managing smart devices — cameras, inside/outside lights, door locks, and a general devices list.

---

## Features

- **Login system** — user authentication (demo credentials below)
- **Camera management** — add, view, and delete security cameras
- **Light control** — manage inside and outside smart lights
- **Door locks** — control smart door locks
- **Device registry** — general device list with SQLite persistence
- **RecyclerView UI** — Material Design list interfaces

---

## Tech stack

- Kotlin
- Android SDK (minSdk 24, targetSdk 33, compileSdk 34)
- AndroidX (AppCompat, Material, ConstraintLayout)
- SQLite (custom `SQLiteOpenHelper` classes)

---

## Quick start

### Prerequisites

- Android Studio (Hedgehog or newer)
- Android SDK API 33–34

### Install and run

```bash
git clone https://github.com/Kaireega/IOT.git
```

1. Open the `IOT/` folder in Android Studio
2. Let Gradle sync
3. Build → Rebuild Project
4. Run on emulator or physical device (API 24+)

### Demo credentials

| Field | Value |
|-------|-------|
| Username | `user` |
| Password | `1234` |

---

## Project structure

```
IOT/
├── app/src/main/
│   ├── java/com/example/iot/
│   │   ├── LoginActivity.kt, MainMenuActivity.kt
│   │   ├── Cameras.kt, InsideLights.kt, OutsideLights.kt
│   │   ├── LockDoors.kt, Devices.kt
│   │   └── *Model.kt, *Adapter.kt, *DBHelper.kt
│   └── res/layout/, res/values/
├── build.gradle.kts
└── settings.gradle.kts
```

---

## Future enhancements

- Real device API integration (MQTT, Zigbee, Z-Wave)
- User registration with SQLite-backed auth
- Push notifications for device events
- Dark mode support

---

## Author

**Kai'ree Gay** — [GitHub](https://github.com/Kaireega)
