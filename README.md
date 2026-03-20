# Simulation-of-1kW-Solar-PV-powered-DC-DC-converter-under-open-loop-condition
## Aim:
To model and design a 1kW solar photovoltaic system using MATLAB Simulation and obtain the current, voltage, power values and solar PV characteristics curves.
## Software Tool Used:
MATLAB 2021 or above

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
3. Connect the thirty-six solar cells in series with common irradiation and make it as a 
subsystem to form a panel.
4. Form similar six panel and connect them in series to form an array with single irradiance 
input.
5. Create a subsystem for the six panels.
6. Connect the constant block with a value of 687 to the irradiance input through PS 
converter.
7. From the output of the solar array connect a current sensor in series to the positive 
terminal and voltage sensor across the terminals.
8. Connect a variable resistor across the solar pv array terminal.
9. Connect a ramp signal to the variable resistor through the PS connector.
10. Using Simulink converter, connect the terminals of the current sensor and voltage sensor 
to the scope to record the graph.
11. Use divide block and convert to multiplication operation and multiply the current and 
voltage outputs to get the power output.
12. Set the minimum and maximum range in X-Y graph to obtain the IV and PV 
characteristics
   
## Simulation diagram:
<img width="1839" height="820" alt="Screenshot 2026-03-20 171549" src="https://github.com/user-attachments/assets/f6d28c6f-f70a-4433-aa6b-03e5393b1b87" />
<img width="730" height="776" alt="Screenshot 2026-03-20 171304" src="https://github.com/user-attachments/assets/dc282803-9357-4690-8281-b82b6340b63d" />
## Output graph:
<img width="1814" height="812" alt="Screenshot 2026-03-20 171429" src="https://github.com/user-attachments/assets/d020aaca-6f3f-472e-9d14-0c03b6aa2578" />
<img width="1828" height="814" alt="Screenshot 2026-03-20 171444" src="https://github.com/user-attachments/assets/98a9edfa-88fe-41da-856c-d34a06c2732a" />

## Tabulation:

