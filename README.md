# UART Transmitter & Receiver (Verilog)

## 📌 Overview
This project implements a **Universal Asynchronous Receiver-Transmitter (UART)** using Verilog. It includes both **UART Transmitter (TX)** and **UART Receiver (RX)** modules, enabling serial communication between digital systems without a shared clock.

The design was simulated and verified using testbenches to ensure accurate data transmission and reception.

---

## ⚙️ Features
- Full-duplex UART communication (TX & RX)
- Configurable baud rate generation
- Start bit, data bits, and stop bit handling
- Serial-to-parallel (RX) and parallel-to-serial (TX) conversion
- Error-free data transmission verification via simulation

---

## 🧠 Design Details

### 🔹 UART Transmitter (TX)
- Accepts 8-bit parallel input data
- Adds:
  - Start bit (0)
  - Stop bit (1)
- Converts parallel data into serial output
- Controlled using a finite state machine (FSM)

### 🔹 UART Receiver (RX)
- Samples incoming serial data based on baud rate
- Detects start bit and reconstructs 8-bit data
- Validates stop bit
- Outputs received parallel data

---

## 🏗️ Architecture
- Baud Rate Generator
- Transmitter FSM
- Receiver FSM
- Shift Registers for data handling

---

## 🧪 Simulation & Verification
- Testbench created to simulate UART communication
- Verified:
  - Correct transmission of data bits
  - Accurate timing based on baud rate
  - Proper detection of start/stop bits
- Waveforms analyzed using simulation tools (e.g., Vivado)

---

## 🛠️ Tools Used
- **Language:** Verilog HDL  
- **Simulator:** Xilinx Vivado / ModelSim  
- **Waveform Viewer:** Vivado Simulator  

---

## 📂 Project Structure
