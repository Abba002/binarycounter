# 🔢 Binary to Hex Counter – FPGA Verilog Project

## 📌 Project Overview

The **Binary to Hex Counter** is an FPGA-based project that allows users to convert a **4-bit binary input (from switches) into its corresponding hexadecimal value** and display it on a **seven-segment display**.

Each switch (`sw[3:0]`) represents a **binary digit**, and the corresponding **hexadecimal value (`0-F`)** is shown in real-time on the **seven-segment display**.

This project demonstrates **binary-to-hex conversion, seven-segment display control, and FPGA input handling**.

---

## 🚀 Features

- 🎚️ **Binary to Hexadecimal Conversion** – Converts a 4-bit binary input into a hexadecimal number (`0-F`).
- 🖥️ **Seven-Segment Display Output** – Displays the hexadecimal value of the binary input.
- 🎛️ **Switch-Controlled Input** – Users can set a 4-bit binary number using FPGA switches (`sw[3:0]`).
- 🔧 **Single-Digit Display** – Only one seven-segment display is used (`an[0]`).
- 💡 **Real-Time Display Updates** – Output updates dynamically as switch inputs change.

---

## 🛠️ Tech Stack

| Component            | Technology Used |
|----------------------|----------------|
| **Programming Language** | Verilog |
| **FPGA Board**       | Nexys A7 |
| **Clock Speed**      | 100 MHz |
| **Constraints File** | `.xdc` for pin mapping |
| **Development Tool** | Xilinx Vivado |

---

## 📂 Installation & Setup

### 1️⃣ **Clone the Repository**
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/Binary-to-Hex-Counter.git
```
### 2️⃣ Navigate to the Project Directory
```sh
cd Binary-to-Hex-Counter
```

## 📂 Installation & Setup

### 3️⃣ **Open in Vivado**
- **Open Vivado** and **create a new project**.
- **Add the Verilog source files** (`top_module.v`, `hex7seg.v`).
- **Add the Nexys A7 constraints file** (`.xdc`) for proper pin mapping.

### 4️⃣ **Run Synthesis, Implementation, and Bitstream Generation**
- **Synthesize the design** (`Run Synthesis`).
- **Implement the design** (`Run Implementation`).
- **Generate the Bitstream** (`Generate Bitstream`).
- **Program the FPGA** using **Vivado Hardware Manager**.

---

## 📜 Usage

### **1️⃣ Start the Counter**
- **Toggle the switches (`sw[3:0]`)** to set a 4-bit binary value.
- **The corresponding hexadecimal value (`0-F`) is displayed** on the seven-segment display.

### **2️⃣ Display Behavior**
| **Binary Input** | **Displayed Value** |
|-----------------|-----------------|
| `0000` (`0`) | Displays `0` |
| `1001` (`9`) | Displays `9` |
| `1010` (`10`) | Displays `A` |
| `1111` (`15`) | Displays `F` |

