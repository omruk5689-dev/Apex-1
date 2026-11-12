# Apex-1
### F1-Inspired High-Speed Line-Following Robot

Apex-1 is a custom-designed, Formula 1-inspired line-following robot built around a PCB designed from scratch. The goal is to bring the robot's main electronics together on a single compact board instead of relying on separate development boards and modules.
<img width="2160" height="3022" alt="3D_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/991eec8a-7ed5-4a28-9029-770e83538235" />
It combines an STM32 microcontroller, motor control, power management and sensor interfaces in a custom-shaped PCB, with an emphasis on functionality, compactness and beginner-friendly assembly.

## Technical Details

| Specification | Details |
|---|---|
| Project | Apex-1 |
| Designed by | Omer |
| PCB Design Software | EasyEDA Pro |
| Development Time | 12 Hours |
| Microcontroller | STM32F103RBT7 |
| Motor Driver | TB6612FNG |
| Display | OLED |
| Sensors | IR Sensors |
| Power Management | Buck Converter |
| PCB Design | Custom Formula 1-inspired PCB |

## Hardware Features

- **STM32F103RBT7:** Main controller for processing sensor inputs and managing robot movement.
- **TB6612FNG:** Dual motor driver for controlling the robot's motors.
- **Buck Converter:** Steps down the battery voltage to the required operating voltage.
- **IR Sensors:** Used to detect the line and provide feedback for navigation.
- **OLED Display:** Provides a small interface for displaying information and debugging.
- **Power Management:** Integrated voltage regulation and power distribution.
- **User Controls:** Three onboard push buttons.
- **Debug Interface:** SWD connections for programming and debugging the STM32.
- **Custom PCB:** Formula 1-inspired board shape with integrated electronic sections.

## PCB Design

Apex-1 features a custom Formula 1-inspired PCB silhouette instead of a conventional rectangular board. The elongated body and front-wing-inspired outline give it a distinctive appearance.

The board integrates the microcontroller, motor driver, power management and peripheral connections. I also wanted the design to be approachable for beginners, so I focused on using through-hole components wherever practical to make assembly, inspection and repairs easier.

## Short Build Guide

1. **PCB Assembly:** Solder the STM32, motor driver, buck converter and supporting components onto the PCB.
2. **Power Setup:** Connect the battery input and verify the regulated voltage outputs before powering the other sections.
3. **Connect Peripherals:** Attach the IR sensors, OLED display and motors to their respective connectors.
4. **Programming:** Connect the SWD debug interface and flash the firmware onto the STM32.
5. **Testing:** Check sensor readings, OLED output and individual motor operation before testing the complete line-following system.


<img width="3332" height="2362" alt="SCH_Schematic1_2-SENSORS_2026-11-08" src="https://github.com/user-attachments/assets/ea81d6df-6b83-4533-95d6-7ce9e9e7628f" />
<img width="3332" height="2362" alt="SCH_Schematic1_1-POWER_2026-11-08" src="https://github.com/user-attachments/assets/c18323f0-2bc9-4d35-bdcd-b4e78f6603cd" />
