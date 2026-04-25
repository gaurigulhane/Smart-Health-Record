# 🏥 Smart Health Record

> **Your Health, Your Records — Secure & Accessible Anytime 🔐**

[![Platform](https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android)](https://android.com)
[![Language](https://img.shields.io/badge/Language-Java%20%7C%20Kotlin-blue?style=for-the-badge)](https://kotlinlang.org)
[![Database](https://img.shields.io/badge/Database-SQLite-orange?style=for-the-badge)](https://sqlite.org)
[![Version](https://img.shields.io/badge/Version-1.0-orange?style=for-the-badge)](#)
[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)

---

## 📖 About

**Smart Health Record** is an Android application designed to help individuals securely manage and track their personal health information. It provides a centralized digital health diary — allowing users to log vital stats, track medications, set health reminders, and monitor trends over time — all protected behind a secure 4-digit PIN.

Built with simplicity and privacy in mind, this app eliminates the hassle of paper records and scattered health notes by consolidating everything into one organized, accessible mobile app.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🧾 **Health Records** | Add, view, and manage personal health history |
| 💊 **Medication Tracker** | Log prescriptions and medication schedules |
| 📊 **Vital Monitoring** | Track BP, Blood Sugar, Weight, and more |
| 🔔 **Reminders & Alerts** | Set custom health reminders and notifications |
| 🔐 **Secure PIN Login** | 4-digit PIN-based authentication for privacy |
| 📈 **Trends & History** | Visualize health data over time with charts |
| 👤 **Profile Management** | Edit profile, backup, and restore health data |

---

## 📱 APK Download

[![Download APK](https://img.shields.io/badge/Download-APK-brightgreen?style=for-the-badge&logo=android)](https://github.com/gaurigulhane/Smart-Health-Record/blob/main/app-debug.apk)

**Installation Steps:**
1. Download the APK from the link above
2. On your Android device, go to **Settings → Security**
3. Enable **"Install from Unknown Sources"**
4. Locate the downloaded APK and tap to install
5. Open the app and set up your 4-digit PIN to get started

---

## 🔄 Application Flowchart

<div align="center">
  <img width="680" alt="Smart Health Record Flowchart" src="https://github.com/user-attachments/assets/68c5af66-f861-4950-91f0-5e5a6fea5603" />
</div>

---

## 🗺️ Detailed Flow Diagram

```
[APP LAUNCH]
     │
     ├──► [First Launch?]
     │         ├──YES──► [Create Profile] ──► [Set 4-digit PIN] ──►┐
     │         └──NO───► [PIN Entry Screen] ──────────────────────►┤
     │                                                              │
     └──────────────────────────────────────────────────────────►[DASHBOARD]
                                                                    │
          ┌─────────────────────────────────────────────────────────┤
          │                                                         │
     [HEALTH RECORDS]                                    [VITALS TRACKER]
          │                                                         │
          ├── Add New Record                            ├── Log Blood Pressure
          ├── View All Records                          ├── Log Blood Sugar
          ├── Search Records                            ├── Log Weight / BMI
          └── Delete Record                             ├── Log Temperature
                                                        └── View Trends/Charts
          │
     [MEDICATIONS]                                   [REMINDERS & ALERTS]
          │                                                         │
          ├── Add Medication                           ├── Set Medication Reminder
          ├── Edit / Update                            ├── Set Appointment Alert
          ├── Track Schedule                           ├── Custom Notifications
          └── Mark as Taken                            └── Manage All Reminders
          │
     [PROFILE & SETTINGS]
          │
          ├── Edit Personal Info
          ├── Change PIN
          ├── Backup Data
          └── Restore Data
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Java / Kotlin** | Core Android development |
| **Android SDK** | Application framework |
| **SQLite** | Local on-device database |
| **Android Studio** | IDE and development environment |
| **SharedPreferences** | PIN storage and user preferences |
| **MPAndroidChart** | Health trend charts and visualizations |

---

## 📂 Project Structure

```
Smart-Health-Record/
│
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/smarthealthrecord/
│   │       │       ├── activities/       # UI screens (Login, Dashboard, etc.)
│   │       │       ├── adapters/         # RecyclerView adapters
│   │       │       ├── database/         # SQLite DB helper & queries
│   │       │       ├── models/           # Data models (Record, Medication, Vital)
│   │       │       └── utils/            # Helper classes, constants
│   │       ├── res/
│   │       │   ├── layout/               # XML layout files
│   │       │   ├── drawable/             # Icons and graphics
│   │       │   └── values/               # Colors, strings, themes
│   │       └── AndroidManifest.xml
│   └── build.gradle
│
├── app-debug.apk                          # Compiled debug APK
├── Smart Health Record_Final.zip         # Full project source zip
└── README.md
```

---

## 🔐 Security

- All health data is stored **locally on the device** using SQLite — no cloud sync, no data sharing.
- Access protected by a **4-digit PIN** set by the user at first launch.
- No personal data is transmitted to any external server.

---

## 🚀 Getting Started (Development)

```bash
# 1. Clone the repository
git clone https://github.com/gaurigulhane/Smart-Health-Record.git

# 2. Open in Android Studio
#    File → Open → Select the cloned folder

# 3. Sync Gradle dependencies
#    Click "Sync Now" when prompted

# 4. Run on emulator or connected Android device
#    Click ▶ Run or use Shift + F10
```

**Requirements:**
- Android Studio Hedgehog (or newer)
- Android SDK 21+ (Android 5.0 Lollipop and above)
- JDK 11 or higher

---

## 📦 Release Info

| Property | Value |
|---|---|
| **Version** | v1.0 |
| **Platform** | Android |
| **Min SDK** | API 21 (Android 5.0) |
| **Target SDK** | API 33 (Android 13) |
| **Build Type** | Debug |

---

## 🔮 Future Enhancements

- [ ] Cloud backup via Firebase or Google Drive
- [ ] Doctor visit history and reports section
- [ ] Export health records as PDF
- [ ] Biometric authentication (Fingerprint/Face ID)
- [ ] Multi-user / family profile support
- [ ] Dark mode support

---

## 📌 About the Project

This project was developed for **learning and demonstration purposes**, showcasing end-to-end Android app development — from UI design to local database management — with a focus on a practical real-world use case: personal health record management.

---

## 👩‍💻 Author

**Gauri Gulhane**

[![GitHub](https://img.shields.io/badge/GitHub-gaurigulhane-black?style=flat-square&logo=github)](https://github.com/gaurigulhane)

---

## ⭐ Support

If you find this project helpful:

- ⭐ **Star** this repository
- 🍴 **Fork** it to build your own version
- 📢 **Share** it with others who might find it useful

---



*Made with ❤️ for better personal health management*
