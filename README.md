# Digital Safe Lock System

![image](https://github.com/A-Alashker/Binary-Lock-/blob/main/Binary%20Lock%20Design.jpg?raw=true)


## Description

This project implements a **digital lock circuit** using logic gates and flip-flops in **Proteus ISIS**. The lock accepts a **binary passcode**, compares it with a **preset code**, and takes an action depending on the correctness of the input. The design includes logic to **block further entries** after **three successive incorrect attempts**.

## Features

- ✅ Accepts a 4-bit binary passcode.
- 🔐 Compares input with a preset 4-bit code.
- ✅ Grants access (green LED) if the code is correct.
- ❌ Denies access (red LED) if the code is incorrect.
- 🚫 After 3 consecutive incorrect attempts, the lock is **disabled** and will **not accept new inputs**.
- 🧠 Implemented using:
  - Flip-Flops (7474)
  - Logic gates (AND 7408, OR 7432, XOR 7486, XNOR 4070)
  - Multiplexers (74157)
  - LED indicators
  - Logic probes and switches

## Components Used For Hardware

![image](https://github.com/TheBestPG22/Binary-Lock-/blob/2558786a516f23166f4363b6bc67b5b41a83870a/Logic%20Gates%20Hardware.jpg)


| Component | Function |
|----------|----------|
| 7474 D Flip-Flops | Store input bits and attempt count |
| 74157 Multiplexers | Code selection and comparison |
| 4070 XNOR Gates | Bitwise comparison between input and preset |
| 7408 AND Gates | Logic control for enabling actions |
| 7432 OR Gates | Combination logic |
| LEDs | Visual indicators for success/failure |
| LogicState & Switches | User input interface |

## Usage

1. Set the desired 4-bit passcode via logic switches.
2. Each clock pulse submits a trial.
3. The circuit compares the code:
   - If **correct**, the green LED lights up.
   - If **incorrect**, the red LED lights up and the failure counter increases.
4. After **3 failed attempts**, input is permanently locked and ignored.

## Simulation

The circuit is designed and tested in **Proteus ISIS Professional**. Ensure all required ICs are included and connected properly to observe correct functionality.



