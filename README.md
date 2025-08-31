# 7-Segment Display Driver (Verilog)

## Description
This project implements a **7-segment display driver** in Verilog. It converts a 4-bit binary input into the corresponding **7-segment display output**. The design supports hexadecimal inputs (0-F) and is compatible with **common-cathode 7-segment displays**.  

The project demonstrates:
- Mapping binary inputs to display segments
- Using combinational logic
- Simulation with waveform visualization

---

## Features
- Supports all 16 hexadecimal inputs (0–F)
- Outputs correct segment pattern for display
- Testbench prints console output for verification
- Compatible with GTKWave/EPWave for waveform visualization

---

## Files
- `txt file ` : Main 7-segment driver module and waveform  
- `png` : Simulation waveform file (generated after running testbench)  

---

## How to Run
1. Open txt file for code and testbench in [EDA Playground](https://www.edaplayground.com/).  
2. Set simulator to **Icarus Verilog**.  
3. Enable **VCD/GTKWave** output.  
4. Click **Run**.  
5. Observe console output (binary input vs segment output) and waveform in GTKWave/EPWave.

---

## Console Output Example
Time Binary Seg[6:0]
10000 0000 0000001
20000 0001 1001111
30000 0010 0010010
40000 0011 0000110
50000 0100 1001100
60000 0101 0100100
70000 0110 0100000
80000 0111 0001111
90000 1000 0000000
100000 1001 0000100
110000 1010 0001000
120000 1011 1100000
130000 1100 0110001
140000 1101 1000010
150000 1110 0110000
160000 1111 0111000


---

## Truth Table

| Binary Input | 7-Segment Output | Display |
|--------------|-----------------|---------|
| 0000         | 0000001          | 0       |
| 0001         | 1001111          | 1       |
| 0010         | 0010010          | 2       |
| 0011         | 0000110          | 3       |
| 0100         | 1001100          | 4       |
| 0101         | 0100100          | 5       |
| 0110         | 0100000          | 6       |
| 0111         | 0001111          | 7       |
| 1000         | 0000000          | 8       |
| 1001         | 0000100          | 9       |
| 1010         | 0001000          | A       |
| 1011         | 1100000          | b       |
| 1100         | 0110001          | C       |
| 1101         | 1000010          | d       |
| 1110         | 0110000          | E       |
| 1111         | 0111000          | F       |

---

## Simulation Waveform (EPWave / GTKWave)
- Signals to view:  
  - `binary_in[3:0]` → input binary values  
  - `seg[6:0]` → segment outputs (a-g)  
- Visualizes which segments turn **ON/OFF** for each binary input.
