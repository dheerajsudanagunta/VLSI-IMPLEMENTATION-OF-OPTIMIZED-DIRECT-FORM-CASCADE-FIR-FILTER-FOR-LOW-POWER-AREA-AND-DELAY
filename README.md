# VLSI Implementation of Optimized Direct & Cascade FIR Filter

## 📌 Project Overview
This repository contains the academic project **“VLSI Implementation of Optimized Direct Form & Cascade FIR Filter for Low Power, Area, and Delay”**, developed as part of the **Bachelor of Technology in Electronics and Communication Engineering** at **VIT Chennai**.

The project focuses on designing and evaluating **16th-order FIR filters** using different combinations of **multipliers** and **adders** to optimize:
- 🔋 Power consumption  
- 🧠 Hardware area (LUT usage)  
- ⏱️ Timing delay (Worst Negative Slack)

Both **Direct Form** and **Cascade Form** FIR architectures are implemented and compared.

---

## 🎯 Objectives
- Design FIR filters using **Verilog HDL**
- Compare **Direct** and **Cascade** FIR architectures
- Analyze different **multiplier** and **adder** combinations
- Optimize FIR filter performance for **low power, low area, and minimal delay**
- Validate designs using **MATLAB** and **Xilinx Vivado**

---

## 🛠 Tools & Technologies
- **HDL**: Verilog  
- **Simulation & Synthesis**: Xilinx Vivado 2021.2  
- **Signal Generation**: MATLAB (Filter Builder – Equiripple Method)  
- **Hardware Target**: FPGA (RTL-based design)

---

## 🔢 FIR Filter Architectures
### 1. Direct Form FIR Filter
- Straightforward implementation
- Higher hardware usage for higher-order filters

### 2. Cascade Form FIR Filter
- Higher-order filter realized using lower-order sections
- Improved numerical stability
- Better delay optimization in some configurations

---

## ✖ Multipliers Implemented
- Booth Multiplier  
- Array Multiplier  
- Vedic Multiplier  

---

## ➕ Adders Implemented
- Ripple Carry Adder (RCA)
- Carry Select Adder (CSA)
- Carry Look-Ahead Adder (CLA)
- Carry Skip Adder (CSIA)
- Kogge-Stone Adder
- Brent-Kung Adder
- Han-Carlson Adder
- Harris Adder
- Knowles Adder
- Ladner-Fischer Adder
- Sklansky Adder

---

## 📊 Performance Metrics
The following parameters were extracted from Vivado implementation reports:
- **Area** → Number of LUTs
- **Power** → On-chip power consumption (W)
- **Delay** → Worst Negative Slack (ns)

### Key Findings
#### ✅ Direct Form
- **Least Area**: Array Multiplier + Ripple Carry Adder  
- **Least Power**: Array Multiplier + Carry Look-Ahead Adder  
- **Least Delay**: Booth Multiplier + Knowles Adder  

#### ✅ Cascade Form
- **Least Area**: Array Multiplier + Carry Skip Adder  
- **Least Power**: Array Multiplier + Carry Select Adder  
- **Least Delay**: Booth Multiplier + Knowles Adder  

---

