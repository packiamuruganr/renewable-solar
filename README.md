# Exp:1 MODELLING AND SIMULATION OF 1kW SOLAR PHOTOVOLTAIC ARRAY  

---

## Aim:
To model and design a 1kW solar photovoltaic system using MATLAB Simulation and obtain the current, voltage, power values and solar PV characteristics curves.

---

## Software Tool Used:
- MATLAB 2021 or above  

---

## Modelling Parameters:

### Solar PV:

| S.No | Parameters | Value |
|------|-----------|------|
| 1 | No. of solar cells | 216 |
| 2 | No. of series cells per panel | 36 |
| 3 | Short circuit current per panel | 2.54A |
| 4 | Open circuit voltage per cell | 21.80V |
| 5 | Irradiance | 1000 W/m2 |
| 6 | Quality factor | 1.6 |
| 7 | Cell resistance (series) | 5.10mΩ |
| 8 | Temperature at STC | 250C |
| 9 | Resistive load | 10Ω |

---

## Theory:

The theory of solar cells explains the process by which light energy in photons is converted into electric current when the photons strike a suitable semiconductor device. The theoretical studies are of practical use because they predict the fundamental limits of a solar cell, and give guidance on the phenomena that contribute to losses and solar cell efficiency. Photons in sunlight hit the solar panel and are absorbed by semi-conducting materials.  

Electrons (negatively charged) are knocked loose from their atoms as they are excited. Due to their special structure and the materials in solar cells, the electrons are only allowed to move in a single direction. The electronic structure of the materials is very important for the process to work, and often silicon incorporating small amounts of boron or phosphorus is used in different layers. An array of solar cells converts solar energy into a usable amount of direct current (DC) electricity.  

The photon can pass straight through the silicon — this (generally) happens for lower energy photons. The photon can reflect off the surface. The photon can be absorbed by the silicon if the photon energy is higher than the silicon band gap value. This generates an electron-hole pair and sometimes heat depending on the band structure.  

## Simulation Diagram:
<img width="1839" height="820" alt="Screenshot 2026-03-20 171549" src="https://github.com/user-attachments/assets/f6d28c6f-f70a-4433-aa6b-03e5393b1b87" />
<img width="730" height="776" alt="Screenshot 2026-03-20 171304" src="https://github.com/user-attachments/assets/dc282803-9357-4690-8281-b82b6340b63d" />

## Tabulation:

| S.No | Short Circuit Current, Isc(A) | Open Circuit Voltage, Voc(V) | Solar Current, Ipv(A) | Solar Voltage, Vpv(V) | Solar Power, Ppv(W) |
|------|------------------------------|-----------------------------|----------------------|----------------------|--------------------|
|   1  |            2.54              |           21.80             |       2.3            |        8             |      19            |

## Procedure:

1. Open MATLAB  
2. From Simulink library browser, pick the following components  
   a. solar cell  
   b. constant  
   c. PS converter, S converter  
   d. Current sensor, voltage sensor  
   e. Variable resistor  
   f. Ramp  
   g. Scope, XY graph  

3. Connect the thirty-six solar cells in series with common irradiation and make it as a subsystem to form a panel.  
4. Form similar six panel and connect them in series to form an array with single irradiance input.  
5. Create a subsystem for the six panels.  
6. Connect the constant block with a value of 687 to the irradiance input through PS converter.  
7. From the output of the solar array connect a current sensor in series to the positive terminal and voltage sensor across the terminals.  
8. Connect a variable resistor across the solar pv array terminal.  
9. Connect a ramp signal to the variable resistor through the PS connector.  
10. Using Simulink converter, connect the terminals of the current sensor and voltage sensor to the scope to record the graph.  
11. Use divide block and convert to multiplication operation and multiply the current and voltage outputs to get the power output.  
12. Set the minimum and maximum range in X-Y graph to obtain the IV and PV characteristics.  


## OUTPUT WAVEFORM:
 <img width="1814" height="812" alt="Screenshot 2026-03-20 171429" src="https://github.com/user-attachments/assets/d020aaca-6f3f-472e-9d14-0c03b6aa2578" />
 <img width="1828" height="814" alt="Screenshot 2026-03-20 171444" src="https://github.com/user-attachments/assets/98a9edfa-88fe-41da-856c-d34a06c2732a" />
 <img width="1900" height="883" alt="Screenshot 2026-03-18 153902" src="https://github.com/user-attachments/assets/3d6a04df-f82e-432e-acb4-f513494cec31" />

## Result:

Thus, the solar PV energy system is simulated using MATLAB and the I-V and P-V graphs are determined for the given panel rating.

