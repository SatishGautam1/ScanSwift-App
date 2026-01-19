# ScanSwift 🔍

ScanSwift is a high-performance, professional-grade Android application designed for seamless QR code and barcode scanning and generation. Built with a focus on speed, privacy, and user experience, it includes "Smart Parsing" logic to extract exactly what you need.


---
## 🌟 Key Features

- **Smart Scanner:** Uses Google ML Kit for lightning-fast detection of QR codes and 1-D/2-D barcodes.
- **Smart Copy Logic:** - **WiFi:** Automatically extracts and copies only the password.
    - **Finance:** Identifies UPI/Banking QRs and extracts Account IDs/Payee addresses.
    - **Websites:** Detects URLs and offers a one-tap open feature.
- **Professional Generator:** Create custom QR codes for text or URLs.
- **Dedicated Storage:** Saves generated and scanned images into a professional `/Pictures/ScanSwift` folder using Scoped Storage.
- **Complete History:** Local database to keep track of all your scans and generations.
- **Modern UI/UX:**
    - Android 12+ Splash Screen API support.
    - Haptic feedback (vibration and beep) for successful scans.
    - Material 3 design with Bottom Sheet result previews.
---
## 🛠 Tech Stack

- **Language:** Java
- **UI Framework:** Material Design Components (M3)
- **Camera API:** CameraX
- **Scanning Engine:** Google ML Kit (Barcode Scanning)
- **Database:** Room Persistence Library
- **Architecture:** ViewBinding, Repository Pattern
- **Min SDK:** 24 (Android 7.0)
- **Target SDK:** 34 (Android 14 / 2026 Ready)

---

## 📂 Project Structure

```text
com.nighttech.scanswift
├── data/           # Database, Entities, and Repository (Room)
├── scanner/        # CameraX implementation and Image Analysis
├── ui/             # Fragments (Scanner, Generator, Settings) and BottomSheets
└── utils/          # QR Generation helpers and UI utilities
```

---
## 🚀 Getting Started
- **Clone the repository:** ```git clone https://github.com/SatishGautam1/ScanSwift.git```
- **Open in Android Studio:** Ensure you have the latest Iguana or Jellyfish build (2024/2025+).
- **Build & Run:** Connect your device and hit ```Shift + F10```.

---
## 🛡 Permissions
ScanSwift respects user privacy and only requests permissions when necessary:
- ```CAMERA:``` To analyze and scan codes in real-time.
- ```WRITE_EXTERNAL_STORAGE:```(Legacy) For saving QR codes to the gallery on older devices.
- ```VIBRATE:``` For haptic feedback on successful scans.

---

## 📄 License
Distributed under the MIT License. See LICENSE for more information.

---

Developed by **NightTech** (2026)
