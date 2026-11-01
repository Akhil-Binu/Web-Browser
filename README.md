# 🌐 Orbit Browser — Lightweight PyQt5 Desktop Web Navigator

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![GUI: PyQt5](https://img.shields.io/badge/GUI-PyQt5-41CD52.svg?style=for-the-badge&logo=qt&logoColor=white)](https://riverbankcomputing.com/software/pyqt/)
[![Engine: Chromium](https://img.shields.io/badge/Engine-PyQtWebEngine-4285F4.svg?style=for-the-badge&logo=googlechrome&logoColor=white)](https://chromium.googlesource.com/)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-black.svg?style=for-the-badge)](https://github.com/Akhil-Binu/Web-Browser)

<p align="center">
  <b>A minimalist, desktop web browser engineered in Python using the Qt5 application framework and the high-performance Chromium-powered PyQtWebEngine.</b>
</p>

</div>

---

## 📌 Overview

**Orbit Browser** delivers a streamlined web browsing experience focused on speed, transparency, and minimal resource overhead. By leveraging Qt's native event loop and WebEngine widget, it provides full modern web rendering (HTML5, CSS3, JavaScript, WebAssembly) inside a clean, customizable desktop GUI.

---

## ✨ Features

- ⚡ **Chromium-Powered Rendering**: Full support for modern web standards via `PyQtWebEngine`.
- 🧭 **Standard Navigation Suite**:
  - Backward / Forward history navigation.
  - Instant page reload & stop request triggers.
  - Configurable default home page.
- 🔗 **Smart Address Bar**: Real-time URL parsing with automatic protocol completion (`http://` / `https://`).
- 🔒 **Secure Sandbox**: Native process isolation inherited from Qt's Chromium core.
- 🎨 **Minimalist Desktop Footprint**: Ultra-low memory consumption compared to heavy multi-process enterprise browsers.

---

## 🛠️ Prerequisites & Installation

### 1. Prerequisites
Ensure you have Python 3.10 or higher installed:
```bash
python --version
```

### 2. Clone the Repository
```bash
git clone https://github.com/Akhil-Binu/Web-Browser.git
cd Web-Browser
```

### 3. Create a Virtual Environment & Install Dependencies
```bash
# Create isolated environment
python -m venv venv

# Activate environment
# On Windows:
venv\Scripts\activate
# On Linux / macOS:
source venv/bin/activate

# Install PyQt5 and QtWebEngine
pip install PyQt5 PyQtWebEngine
```

---

## 🚀 Running the Browser

Execute the main application script:

```bash
python main.py
```

---

## 🏗️ Architecture & Qt Event Loop

```
 ┌────────────────────────────────────────────────────────┐
 │                      QMainWindow                       │
 │  ┌──────────────────────────────────────────────────┐  │
 │  │      QToolBar (Back, Forward, Reload, Home)       │  │
 │  │      QLineEdit (Smart URL Bar)                   │  │
 │  └──────────────────────────────────────────────────┘  │
 │  ┌──────────────────────────────────────────────────┐  │
 │  │                 QWebEngineView                   │  │
 │  │          (Chromium Rendering Pipeline)           │  │
 │  └──────────────────────────────────────────────────┘  │
 │  ┌──────────────────────────────────────────────────┐  │
 │  │      QStatusBar (Loading Progress / SSL Status)  │  │
 │  └──────────────────────────────────────────────────┘  │
 └────────────────────────────────────────────────────────┘
```

---

## 📄 License

Distributed under the [MIT License](LICENSE). Created by [Akhil Binu](https://akhilbinu.in/).
