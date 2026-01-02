# 🔋 +5V to +3.3V Regulator PCB (Altium Designer)
This project is a simple and efficient **+5V to +3.3V linear regulator circuit** designed in **Altium Designer**.  
It uses the **MIC5317-3.3YM5-TR** Low Dropout (LDO) voltage regulator to provide a clean 3.3V output for powering microcontrollers, sensors, and logic devices from a 5V supply.

---

## ⚙️ Features

- **Input Voltage:** +5V DC  
- **Output Voltage:** +3.3V DC  
- **Regulator IC:** MIC5317-3.3YM5-TR (Low Dropout Regulator)  
- **Input Capacitor:** 1 µF  
- **Output Capacitor:** 1 µF  
- **Connectors:** JST SM02B-GHS-TB (2-pin input and output)  
- **Compact and low-noise PCB layout**  
- Designed using **Altium Designer**  

---

## Contents
- Schematic and PCB design files (`.SchDoc`, `.PcbDoc`)
- Gerber files for fabrication
- Reports and documentation

## Software
Designed using **Altium Designer**.

## Schematic Preview
The circuit uses the **MIC5317-3.3YM5-TR** low-dropout voltage regulator to convert +5V input to +3.3V output.
<img width="1280" height="485" alt="image" src="https://github.com/user-attachments/assets/2cb0688a-a649-4987-be42-b90927cba3ba" />


## PCB 2d Preview
PCB Top View <img width="1089" height="533" alt="image" src="https://github.com/user-attachments/assets/01920388-99ad-4a3b-b064-b6f611876e8d" />


## PCB 3d Preview
PCB Top View <img width="987" height="491" alt="image" src="https://github.com/user-attachments/assets/de999a83-e60a-4d3a-aa13-035497fa2033" />

## Design Decisions 

- Choose MIC5317 for its low dropout voltage and stable operation at low load currents.

- 1 µF input and output capacitors were selected as per datasheet recommendations to ensure stability and minimize output noise.

- Short trace lengths were maintained between the regulator and output capacitor to reduce transient response issues.

- Ground plane continuity was prioritized to minimize noise and improve thermal performance.

- Connector placement was optimized for easy integration into embedded prototype boards.

 ## ⚠️ Known Limitations & Future Improvements 

- As a linear regulator, efficiency drops significantly when stepping down from 5V to 3.3V at higher load currents.

- Thermal performance may degrade under continuous high-current operation.

- No EMI filtering is included beyond basic decoupling.

- Future iteration ideas:

  - Replace LDO with a buck converter for higher efficiency

  - Add thermal vias under the regulator

  - Include optional EMI filtering on input/output
