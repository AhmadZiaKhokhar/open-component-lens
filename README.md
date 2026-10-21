# Open Component Lens v3.1 Pro 🔬⚡

An encrypted, serverless electronic component inventory, project tracker, and **Gemini AI** lab assistant designed for hardware hackers, makers, and embedded engineers.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-v3.1%20Pro-emerald.svg)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.x-38bdf8.svg)
![Gemini AI](https://img.shields.io/badge/AI-Gemini%201.5%20Flash-8e44ad.svg)

---

## 🌟 Key Features

* **🔍 AI-Powered Lens Scanner:** Snap or upload component photos. Powered by **Gemini 1.5 Flash**, it automatically extracts part numbers, operational voltage ranges ($V_{\min} - V_{\max}$), datasheets, and categories.
* **⚠️ Dynamic Stock Shortage Engine:** Real-time inventory monitoring that cross-references active project demands against current stock quantities.
* **🛠️ Isolated Project Playground:** Dedicated workspace per project build featuring checklist tasks, linked components, and a custom Gemini AI Lab Coach.
* **🔒 Enterprise-Grade Client-Side Security:** Zero backend database needed. Secrets (Gemini API keys, cloud master tokens) are encrypted locally using **AES-256** secured with a Master PIN.
* **☁️ Cloud Sync & Persistent Storage:** Seamless REST integration with JSONBin for multi-device sync without setup hassle.
* **🎨 Modern Tech-Focused Glassmorphism UI:** Built with dark-mode aesthetic, responsive layouts, and industry-standard typography for high legibility in lab environments.

---

## 🛠️ Architecture Overview

```
+-----------------------------------------------------------------+
|                       Open Component Lens                       |
+-----------------------------------------------------------------+
          |                                       |
   [ Client-Side AES-256 ]                 [ AI Lens Engine ]
   (Master PIN Encryption)                 (Gemini 1.5 Flash API)
          |                                       |
   [ JSONBin REST Sync ]                  [ Webcam / File Stream ]
```

---

## 🚀 Quick Start

Since **Open Component Lens** is fully client-side and serverless, no node server or build pipeline is strictly required to run it locally.

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/open-component-lens.git
cd open-component-lens
```

### 2. Run the App
Simply open `index.html` in your favorite web browser or start a lightweight HTTP server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js serve
npx serve .
```

Navigate to `http://localhost:8000`.

---

## 🔐 Security & API Configuration

1. Click the **Security / Shield** icon in the header.
2. Set up your **Master PIN**.
3. Optionally enter your **Gemini API Key** (from Google AI Studio) to enable live vision identification and the AI Lab Coach.
4. (Optional) Provide your **JSONBin Bin ID & Master Key** to synchronize inventory across devices.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
