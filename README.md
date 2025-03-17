# 🔥 Internal Combustion Engine Simulation  
This project simulates the operation of an **internal combustion petrol engine** in C++. The simulation models engine dynamics such as **piston movement, RPM changes, fuel combustion**, and speed control.  

🚀 **Goal**: Provide a simple yet interactive way to understand how a petrol engine works through a **C++ terminal-based simulation**.  

---

## **🛠 Features**  
✔️ Simulates the **four-stroke cycle** (Intake, Compression, Power, Exhaust)  
✔️ Adjust **engine speed (RPM)** with interactive controls (`+` and `-` keys)  
✔️ Displays **real-time RPM and fuel consumption**  
✔️ Models **fuel injection, ignition timing, and piston movement**  
✔️ Smooth frame-rate control for a **realistic simulation experience**  

---

## **📦 Requirements**  
### **1️⃣ System Requirements**  
🖥️ Works on **Windows, Linux, and macOS**  
🛠️ Requires a **C++ compiler** (e.g., g++, clang)  

### **2️⃣ Dependencies**  
- `ncurses.h` (For interactive terminal input handling)  
- `iostream`, `cmath`, `thread`, `chrono`  

To install dependencies:  
#### **Linux (Ubuntu/Debian)**  
```bash
sudo apt update && sudo apt install libncurses5-dev

## **🚀 Installation Guide**  
### **🖥️ Windows (Code::Blocks & FreeGLUT)**
#### **1️⃣ Install Code::Blocks (with MinGW)**
1. Download [Code::Blocks](http://www.codeblocks.org/downloads/26) **(with MinGW compiler)**  
2. Install Code::Blocks and ensure it detects the MinGW compiler  

#### **2️⃣ Install FreeGLUT (for 3D Support)**
1. Download **FreeGLUT Windows binaries** from [here](https://www.transmissionzero.co.uk/software/freeglut-devel/)  
2. Extract the ZIP file  
3. Copy:  
   - `freeglut.dll` → `C:\Windows\System32\`  
   - `libfreeglut.a` → `C:\MinGW\lib\`  
   - `freeglut.h` → `C:\MinGW\include\GL\`  

#### **3️⃣ Install Ncurses for Terminal Interaction**  
1. Download [PDCurses](https://pdcurses.org/)  
2. Extract it and copy the `.h` and `.a` files to `C:\MinGW\include\`  

#### **4️⃣ Compile and Run**
1. Open Code::Blocks  
2. Load `main.cpp`  
3. Go to **Settings > Compiler > Linker settings**  
   - Add: `-lglut -lGL -lncurses -lpthread`  
4. Press **Build & Run**  

---

### **🐧 Linux Installation (Ubuntu/Debian)**
```bash
sudo apt update
sudo apt install g++ freeglut3-dev libncurses5-dev
g++ -o engine_sim main.cpp -lglut -lncurses -lpthread
./engine_sim