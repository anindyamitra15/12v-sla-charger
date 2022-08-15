# 12V SLA Battery Charger Solution

12V 7.2Ah Sealed Lead Acid (SLA) batteries are very common. However a few factors should be kept in mind while charging them through a power supply. There should be a charging circuit which roughly charges the battery with a certain charging curve.

# Notes
- Charging Curve for each cell (2.1v nominal) <br>
![Charging Curve for each cell](https://user-images.githubusercontent.com/55695557/184611809-51fbf34d-32c2-4fb5-a518-fec1e4586fb7.jpg)

- Charging Modes
    
    - Bulk Charge:
    Constant current mode - The maximum current is written on the body of the cell, most of them can take upto 1.2A (keeping temperature in mind). However, as a rule of thumb, it is a good practice to keep the charging current at 1/10th of the rated current. So, in this case charging current would roughly be 7.2A/10 = 0.72A = 720mA.

    - Absorption:
    Constant voltage mode - The cycle charge voltage (i.e., 14.2 - 14.4v, or roughly 2.4v per cell) is the voltage to be kept during absorption, for approx. 5hrs.

    - Float (storage):
    Voltage should be dropped to 13.7 - 13.9v) (max. 2.3v per cell) and current should be capped at 1mA.


# Constant Current
- A closed loop system which the desired current at the output, set by a threshold value.

# Constant Voltage
- A closed loop system which the desired voltage at the output, set by a threshold value.

# Analog
- Linear current source
    - Simple - Less components
    - Very little efficiency - heat dissipation
# Digital
- PWM
    - Involving a microcontroller would be most effective
    - needs more components (like an inductor of a certain value etc.) to achieve precision
    - Very efficient

# Schematic

# PCB Layout

# Licensing
Commercial usage is strictly disallowed.