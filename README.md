<h1 align="center">NETnahihai: Offline Map Navigation 🇮🇳</h1>

<p align="center">
  <img align="center" src="app/src/main/res/mipmap-xxxhdpi/ic_launcher.png" alt="NETnahihai App Icon" width="192" height="192">
</p>

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Made%20in-India%20%F0%9F%87%AE%F0%9F%87%B3-FF9933?style=for-the-badge&logoColor=white" alt="Made in India"></a>
  <a href="#"><img src="https://img.shields.io/badge/Lead%20Developer-Krishna-138808?style=for-the-badge" alt="Created by Krishna"></a>
  <a href="#"><img src="https://img.shields.io/badge/Status-Active%20Offline%20Nav-0A52D0?style=for-the-badge" alt="Status"></a>
</p>

<p align="center">
  <strong>NETnahihai is a high-performance offline navigation app for Android. Built for seamless navigation when there is no internet connection ("Net Nahi Hai? No Problem!"), powered by GraphHopper for routing algorithms and MapLibre for crystal-clear offline map rendering.</strong>
</p>

## ✨ Highlights

* 🇮🇳 **Proudly Made in India** — Built for reliability everywhere, even with zero network coverage.
* 📍 **100% Offline Navigation** — View maps, search locations, and navigate turnkey routes with zero mobile data.
* 🚗 **Multi-Profile Routing** — Tailored routing for Car, Motorcycle, and Foot.
* 🔄 **Smart Re-routing** — Auto-recalculates your path when you deviate more than 30m.
* ⚡ **High Efficiency** — Vector tile rendering with MapLibre & compressed offline map packages.

## 📱 Screenshots

<div align="center">
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/1_map.png?raw=true" width="170" vertical-align="middle"/>
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/2_map.png?raw=true" width="170" vertical-align="middle"/>
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/3_map.png?raw=true" width="170" vertical-align="middle"/>
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/4_map.png?raw=true" width="170" vertical-align="middle"/>
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/5_map.png?raw=true" width="170" vertical-align="middle"/>
  <img src="https://github.com/khoa083/mapdata/blob/main/screen/screen-20260421-162624-1776763553324.gif?raw=true" width="200"/>
</div>

## 🚀 Features

* **Complete Offline Directions**: Turn-by-turn navigation without any internet connection.
* **Resumable Map Downloads**: Background download via WorkManager with HTTP-Range support.
* **Storage-Optimized**: Compressed map packages in tar.zst format to save disk space.
* **Interactive Map Controls**: Rotate, pitch, zoom, and 2D/3D compass mode toggles.
* **Dynamic Recalculation**: Off-track detection (> 30m) with fast re-routing.
* **Vehicle & Pedestrian Support**: Car, motorcycle, and walking profiles.
* **POI & Place Search**: Vector-based Point of Interest discovery and hybrid offline search.
* **In-app Update Checker**: Easily stay up to date.

## 📋 Project Status

| Feature | Status |
| :--- | :---: |
| **Lock Screen Navigation** | 🟡 In Progress |
| **Speed Limits** | 🔴 done |
| **Voice Guidance** | 🔴 Planned |

## 👤 Author & Credits

* **Creator & Lead Developer**: **Krishna** 🇮🇳
* **Routing Engine**: [GraphHopper](https://www.graphhopper.com/)
* **Map Rendering**: [MapLibre](https://maplibre.org/)
* **Map Data**: [OpenStreetMap](https://www.openstreetmap.org/) contributors
* **Map Tiles & Hosting**: [OpenFreeMap](https://openfreemap.org/)
* **POI & Geocoding Search**: [Photon](https://photon.komoot.io/)
* Modernized and rewritten using **Clean Architecture**, **MVVM**, **Kotlin**, and **Jetpack Compose**.

## 🏗️ Architecture

The project is built with **Clean Architecture** and follows the **MVVM (Model-View-ViewModel)** pattern to ensure scalability, maintainability, and ease of testing.

* **UI Components**:
    * **Jetpack Compose** (Declarative UI)
    * **Material Design 3**
* **Dependency Injection**: Hilt
* **Asynchronous Processing**: Coroutines & Flow
* **Navigation**: Navigation Compose
* **Local Data**: Room Database & DataStore (Preferences)
* **Remote Data**: Retrofit 2 + OkHttp + Moshi (JSON)
* **Routing Engine**: GraphHopper
* **Map Rendering**: MapLibre Compose
* **Other Libraries**:
    * **WorkManager**: Background tasks processing
    * **Timber**: Advanced logging
    * **Chucker**: In-app HTTP inspection (Debug)
    * **LeakCanary**: Memory leak detection
    * **Konfetti**: Particle system for celebratory effects
    * **Commonmark**: Markdown rendering support

## 🛠️ Build & Setup

### Requirements

* [Android Studio](https://developer.android.com/studio) Ladybug or newer
* Java 21 or higher

### Steps

1. Clone or open the repository:
   ```bash
   cd map-offline-navigation-main
   ```
2. Open the project in Android Studio
3. Sync Gradle and run the app on an Android device or emulator

### Running tests

* Run all unit tests:
  ```bash
  ./gradlew :app:testDebugUnitTest
  ```

* Run Jacoco test coverage:
  ```bash
  ./gradlew :app:jacocoTestReportAll
  ```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Help us improve **NETnahihai: Offline Map Navigation**.

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.
