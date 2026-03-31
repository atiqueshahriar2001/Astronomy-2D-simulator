# 🌌 Astronomy 3D Simulator

A **real-time 3D Solar System simulator** built using **C++ and OpenGL (GLUT)**.
This project visually represents the solar system with animated planets, realistic orbital motion, lighting, and a dynamic starfield.

---

## 🚀 Features

✨ **Core Highlights**

* 🌞 Realistic **Sun** with glowing animation & pulsating rays
* 🪐 **All 8 planets** orbiting with unique speed & distance
* 🌍 **Earth's Moon** with independent orbit
* 💫 **2000+ twinkling stars** for immersive background
* 🌀 **Saturn’s rings** with custom geometry
* 🔄 Toggleable **orbit paths**
* 💡 Dynamic **lighting system** from the Sun
* 🎮 Fully **interactive camera controls**

---

## 🎮 Controls

| Key       | Action                     |
| --------- | -------------------------- |
| `W` / `S` | Move camera up / down      |
| `A` / `D` | Rotate camera left / right |
| `+` / `-` | Zoom in / out              |
| `Space`   | Pause / Resume animation   |
| `O`       | Toggle orbit paths         |
| `L`       | Toggle lighting            |
| `Esc`     | Exit application           |

---

## 🧰 Technologies Used

* **C++**
* **OpenGL**
* **GLU (OpenGL Utility Library)**
* **GLUT / FreeGLUT**

---

## ⚙️ Installation & Build

### 🐧 Linux (GCC)

```bash
g++ main.cpp -o main -lGL -lGLU -lglut -lm
./main
```

---

### 🪟 Windows (MinGW)

```bash
g++ main.cpp -o main.exe -lfreeglut -lopengl32 -lglu32
./main.exe
```

> ⚠️ Ensure **FreeGLUT / GLUT libraries** are properly installed.

---

## 🪐 Planet Configuration

| Planet  | Distance | Radius | Color           |
| ------- | -------- | ------ | --------------- |
| Mercury | 10       | 1.2    | Gray            |
| Venus   | 16       | 1.8    | Tan             |
| Earth   | 24       | 2.0    | Blue 🌍         |
| Mars    | 32       | 1.5    | Red 🔴          |
| Jupiter | 45       | 4.5    | Orange-brown    |
| Saturn  | 58       | 3.8    | Gold 🟡 (rings) |
| Uranus  | 72       | 3.2    | Cyan 🔵         |
| Neptune | 88       | 3.0    | Dark Blue 🔷    |

---

## 📸 Future Improvements (Optional Ideas)

* 🌌 Add **asteroid belt**
* 🌗 Planet **rotation on axis**
* ☄️ Add **comets**
* 🎥 Multiple **camera modes (top view / free fly)**
* 🌍 Realistic **textures (NASA textures)**

---

## 📄 License

This project is provided for:

* 🎓 Educational purposes
* 🧪 Personal experiments


## Here is how to set up the standalone compiler and FreeGLUT.

## Download the Standalone Compiler (WinLibs)

1. Go to WinLibs.com.
2. Scroll down to the "Release" section.
3. Look for UCRT runtime, Win64, and download the Zip archive (e.g., "GCC 14.2.0 + LLVM/Clang...").
4. Extract it: Unzip the folder to a simple location like C:\mingw64.

## Add to Environment Variables

1. Windows needs to know where g++.exe lives.
2. Open the Start Menu, type "Environment Variables", and select Edit the system environment variables.
3. Click Environment Variables > Select Path > Click Edit.
4. Click New and paste: C:\mingw64\bin
5. Click OK on all windows.


## Download & Place FreeGLUT

1. Since you are doing a manual setup, let's put FreeGLUT directly into your compiler folders so you don't have to keep copying files into every new project.
2. Download the freeglut 3.0.0 MSVC Package from Transmission Zero.
3. Move Headers: Copy everything inside the zip's include/GL folder into C:\mingw64\include\GL.
4. Move Libraries: Copy the .lib files from the zip's lib/x64 folder into C:\mingw64\lib.
5. Move the DLL: Copy freeglut.dll from the zip's bin/x64 folder into C:\Windows\System32 (this allows any OpenGL program you write to run globally).

## Download Link(GCC + MinGW)

https://www.winlibs.com

## Download Link (OpenGL + GLUT)

https://www.transmissionzero.co.uk/software/freeglut-devel
