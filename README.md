# Receiver-Sensitivity
# Optical Receiver Sensitivity Analysis

## Objective
Determine the sensitivity of a PIN photodiode-based optical receiver by calculating the minimum received power necessary to achieve a given Q factor. Compare simulation results with those obtained analytically.

---

## Theory
If only thermal noise is considered, the sensitivity of a PIN photodiode-based receiver is:



<img width="1126" height="718" alt="image" src="https://github.com/user-attachments/assets/22298a91-302d-41e4-b254-86c9b8ec704e" />

---

## Calculations
Receiver specifications:

| Parameter                        | Value                          |
|----------------------------------|--------------------------------|
| Operating bit rate               | 2.5 Gb/s                       |
| Bandwidth                        | 1.65 × bit rate                |
| Thermal noise spectral density    | X.Y × 10⁻²² A²/Hz              |
| Desired Q factor                 | 6                              |
| PIN photodiode responsivity      | 1 A/W                          |

> **Note:** X and Y are the last two digits of your student ID.  
> Example: If ID ends with **43**, then ST = 4.3 × 10⁻²² A²/Hz.  

Using the formulas above, calculate the receiver sensitivity.

---

## Layout
The simulation layout consists of:
1. CW laser source  
2. NRZ modulator  
3. Optical attenuator  
4. PIN photodiode with electrical filter  

Settings:
- Responsivity = 1 A/W (default)  
- Dark current = 0  
- ASE noise = off  
- Thermal noise parameter = editable  

Power meters are placed:
- At the modulator output  
- After the attenuator (input to receiver)  

---

## Simulation
Steps:
1. Adjust output power to **0 dBm**.  
2. Set attenuator to **20 dB**.  
3. Run the simulation.  
4. Adjust attenuator until **Q factor = 6.00 ± 0.05**.  

---
### TABULATION
![WhatsApp Image 2026-02-25 at 10 20 20 AM](https://github.com/user-attachments/assets/faae4b4b-5bd3-41fc-8c6d-862f8cf6bc90)

## Report
Your report should include:
- Pre-lab calculations (attach handwritten work if applicable).  
- Screenshots or displays of simulation results:
- Power readings  
- BER analyzer output  
- Eye diagram  
- Discussion of differences between analytical and simulation results.  

---
## RESULT
The simulation result closely matched the analysis value with only minor variation due to filter bandwidth and numerical effects confirming the theoretical receiver sensitivity 
