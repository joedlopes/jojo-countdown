# 🚀 JoJo-Countdown!

> **Keep your tasks and focus on track!**

**JoJo-Countdown!** is a playful and visually engaging productivity timer that helps you stay focused using countdown sessions and break reminders. Built with **JavaScript**, **Bootstrap 5**, and a space-surfing cat mascot, JoJo Countdown turns your task list into a time-managed flow. 


![JoJo Logo](assets/icons/icon.png)


---

## 🛠️ Features

* ⏳ Countdown-based focus sessions
* ⏸️ Break reminders
* 🐱 Mascot animation to keep things fun
* 💡 Built with HTML, CSS, JS, Electron, and Bootstrap

---

## 🧰 Tech Stack

* Electron.js
* Bootstrap
* HTML5 + CSS3
* JavaScript (Vanilla)

---

## 📦 Building the App

You can build JoJo-Countdown! on Linux for both Linux and Windows platforms.

### 📁 Project Setup

```bash
npm install
```

---

### 🐧 Linux Builds

> Ensure required dependencies:

```bash
sudo apt install libfuse2
```

#### `.deb` Package

```bash
npx electron-builder --linux deb
```

#### `.AppImage` Package

```bash
npx electron-builder --linux AppImage
```

#### Unpacked Directory

```bash
npx electron-builder --linux dir
```

#### Manual Packager (Optional)

```bash
electron-packager . JoJoCountdown --platform=linux --arch=x64 --icon=images/icon.png --overwrite
```

---

### 🩟 Windows Builds (from Linux)

> Requires Wine & Mono:

```bash
sudo apt install wine mono-devel nsis
```

#### Installer `.exe`

```bash
npx electron-builder --win nsis
```

#### Portable `.exe`

```bash
npx electron-builder --win portable
```

#### Manual Packager (Optional)

```bash
electron-packager . JoJoCountdown --platform=win32 --arch=x64 --icon=images/icon.png --overwrite
```

---

### 📦 Build All Targets

```bash
npx electron-builder --win --linux
```

> Output files will be in the `dist/` folder.

---

## 📁 Project Structure

```
jojo-countdown/
├── images/
│   └── icon.png / icon.ico
├── index.js
├── package.json
├── dist/
└── ...
```

---

## 📄 License

This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2025 Joed Lopes da Silva

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
