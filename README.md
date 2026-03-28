# TEST-
# 🎓 The Big Six · UPSA Academic Portal

> A secure, cloud-synced academic results portal built for **The Big Six** study group at the University of Professional Studies, Accra (UPSA).

---

## 🌐 Live Demo

👉 [https://cudjoemensah5-lab.github.io/THE-BIG-SIXX-PORTAL/](https://cudjoemensah5-lab.github.io/THE-BIG-SIXX-PORTAL/)

---

## 📌 About

The Big Six Portal was built to solve a real problem — the official UPSA portal is unreliable, often failing to load or losing data on logout. This portal gives study group members a fast, secure, and always-available alternative to view their academic results.

---

## ✨ Features

- 🔐 **Two-role system** — Admin (Teacher) dashboard & Student results viewer
- ☁️ **Firebase Firestore** — Real-time cloud sync across all devices
- 📴 **Offline fallback** — Switches to local storage if Firebase is unavailable
- 📊 **Auto-calculated CGPA** — Grades and classifications computed automatically
- 📈 **Chart.js Analytics** — Visual breakdown of student performance
- 🛡️ **SHA-256 PIN hashing** — Secure admin authentication
- 🔒 **Brute-force lockout** — Admin locked out after 5 failed PIN attempts
- 🔑 **Forced PIN change** — Admin must change default PIN on first login
- 👁️ **Read-only student view** — Students can only view, never edit results
- 📱 **Fully responsive** — Works on mobile, tablet, and desktop

---

## 🛠️ Built With

| Technology | Purpose |
|---|---|
| HTML / CSS / JavaScript | Frontend (single file) |
| Firebase Firestore | Cloud database |
| Chart.js | Results analytics charts |
| Google Fonts (Syne + DM Mono) | Typography |
| GitHub Pages | Hosting & deployment |

---

## 🚀 Deployment (GitHub Pages)

1. Fork or clone this repository
2. Make sure your Firebase project is set up at [console.firebase.google.com](https://console.firebase.google.com)
3. Replace the Firebase config in `index.html` with your own project credentials
4. Push to GitHub and enable **GitHub Pages** from the `main` branch
5. Your portal will be live at `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

---

## 🔧 Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a project and enable **Firestore Database**
3. Add your GitHub Pages URL as an **Authorized Domain**
4. Copy your config and paste it into the `FB_CONFIG` section in `index.html`
5. Set Firestore security rules to allow only authenticated admin writes

---

## 🔐 Security

- Admin PIN is hashed with **SHA-256** before storage — never stored as plain text
- Legacy plain-text PINs are automatically migrated to hashed format on first login
- Default PIN is `123456` — admin is **forced to change it** on first login
- Students have **zero write access** — results are read-only for all student accounts

---

## 👥 Study Group

Built for **The Big Six** — a dedicated study group at UPSA, Accra 🇬🇭

---

## 📄 License

This project is for academic and personal use within The Big Six study group.

---

> *Built with 💚 by The Big Six — UPSA, Accra*
