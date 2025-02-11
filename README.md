# Embedded System Design: LED Control with SPST Switch Using PIC24F04KA200
This repository contains an embedded system project that demonstrates how to control three LEDs (Red, Green, and White) using an SPST switch. The project utilizes the **PIC24F04KA200** microcontroller, **Proteus 8.10** for simulation, and **MPLAB X IDE with XC8 Compiler** for code development.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Software and Tools](#software-and-tools)
- [Dependencies](#dependencies)
- [Authors](#authors)
- [License](#license)

## Project Overview

The project is divided into three main stages:

1. **Hardware and Circuit Design**
   - **Microcontroller Used:** PIC24F04KA200
   - **Circuit Design:** Created using **Proteus 8.10** simulation software.
   - **Connections:**
     - **Switch ON:** Red LED remains ON, Green LED blinks every 3 seconds.
     - **Switch OFF:** White LED turns ON, Red and Green LEDs turn OFF.

2. **Firmware Development**
   - **IDE Used:** MPLAB X IDE
   - **Compiler:** XC8 Compiler
   - **Programming Language:** C
   - **Code Implementation:** LED behavior controlled based on switch state.

3. **Simulation and Testing**
   - **Proteus Simulation:** The Proteus project is used to test the LED switching behavior before real-world implementation.
   - **HEX File Loading:** The compiled `.hex` file is loaded into the microcontroller inside Proteus for simulation.

## **Installation**
### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/Embedded_System_LED_Control.git
cd Embedded_System_LED_Control
```
### **2. Open the Proteus Project**
```bash
# Navigate to the ProteusProject folder
cd ProteusProject
# Open the PIC24F04KA200-SPST-LEDs project file in Proteus
```
### **3. Load the HEX File**
```bash
# In Proteus, double-click the PIC24F04KA200 microcontroller
# In the Program File section, click the folder icon
# Navigate to HexFile/ and select the PIC24F04KA200_SPST_LEDs.production.hex file
```
### **4. Run the Simulation**
```bash
# Click Run Simulation and observe the LED behavior
```

## **Usage**
### **1. Microcontroller Behavior**
```bash
# Switch ON:  
# - Red LED stays ON  
# - Green LED blinks every 3 seconds  

# Switch OFF:  
# - White LED turns ON  
# - Red and Green LEDs turn OFF  
```
### **2. How to Modify the Code**
```bash
# Open the main.c file located in SourceCode/
# Modify the delay times or LED logic as needed
# Recompile the code using MPLAB X IDE
# Generate a new HEX file and update the Proteus simulation
```

## **Software and Tools**
```bash
| Software      | Purpose |
|--------------|---------|
| Proteus 8.10 | Circuit simulation |
| MPLAB X IDE  | Writing and compiling C code |
| XC8 Compiler | Generating HEX files |
```

## **Dependencies**
```bash
# This project requires the following tools:
# - Proteus 8.10 (for circuit design and testing)
# - MPLAB X IDE (for developing and compiling the C code)
# - XC8 Compiler (for compiling the source code)
```

## **Authors**
```bash
# This project was developed by Kaleab Tesfaye
```

## **License**
```bash
# This project is licensed under the MIT License – see the LICENSE file for details.
