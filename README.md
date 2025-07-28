# 🔢 LED 7-Segment Counter: From 0 to 9

Final project for the **Digital Electronics** course – Faculty of Advanced Science and Technology, University of Science and Technology – The University of Danang.

## 📖 Overview

This project aims to **design, simulate, and implement** both a **synchronous** and **asynchronous** up counter that displays numbers from `0` to `9` using a **7-segment LED display**. It includes:

- A debounce circuit for the push-button
- Binary to 7-segment decoder logic
- Simulation using **Proteus**
- Real-world implementation on **breadboard**

**Instructor:** Dr. Lê Quốc Huy  
**Timeline:** April 22, 2024 – May 29, 2024

---

## ⚙️ Features

- ✅ **Synchronous Counter** (all flip-flops share the same clock signal)
- ✅ **Asynchronous Counter** (flip-flops are chained)
- ✅ **7-Segment Decoder** using Karnaugh maps
- ✅ **Debounce circuit** to filter button bounce
- ✅ **Breadboard implementation**
- ✅ **Proteus simulation**

---

## 🧩 Components Used

| Component     | Quantity | Description                |
|---------------|----------|----------------------------|
| CD4069        | 1        | Hex Inverter (NOT Gate)    |
| 74HC08        | 2        | 2-input AND Gates          |
| 74HC11        | 3        | 3-input AND Gates          |
| 74HC21        | 1        | 4-input AND Gates          |
| 74HC32        | 2        | OR Gates                   |
| CD4072        | 1        | Dual 4-input OR Gates      |
| CD4075        | 1        | Triple 3-input OR Gates    |
| 74HC00        | 1        | NAND Gates                 |
| 74LS73        | 4        | JK Flip-Flops              |
| Push Button   | 1        | Clock trigger              |
| Resistors     | Several  | 1kΩ and 10kΩ                |
| 7-Segment LED | 1        | Common Cathode             |
| Breadboard    | 3        | Circuit prototyping        |
| Jumper Wires  | ~7m      | Connections                |

---

## 🛠️ How It Works

### 1. Push Button & Debounce
- The input signal is cleaned using a debounce circuit to ensure stable rising edges to trigger counting.

### 2. Counting Logic
- A 4-bit counter is built using **JK Flip-Flops** (74LS73).
- Two modes implemented:
  - **Synchronous counter**
  - **Asynchronous counter**

### 3. Decoder Logic
- 4-bit binary output is decoded into a 7-segment display pattern (a–g).
- Designed using **Karnaugh Maps** for simplified logic.

---

## 🧪 Simulation

- Designed and simulated using **Proteus Design Suite**.
- Visual confirmation of incrementing numbers upon each button press.
- Simulation files are included in the `/proteus/` directory.

---

## 🔌 Physical Circuit

- Implemented on a **breadboard** using real components.
- Powered with **5V DC**.
- Button press increments display from 0 → 9, then rolls over.

---

## 📂 Project Structure

