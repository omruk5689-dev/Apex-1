# Apex-1
### F1-Inspired High-Speed Line-Following Robot
<img width="2160" height="3022" alt="3D_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/991eec8a-7ed5-4a28-9029-770e83538235" />

Apex-1 is a custom-designed, Formula 1-inspired line-following robot. The idea behind this project was to build a fast and compact robot while designing its electronics from scratch, rather than relying on separate development boards and modules.

| Project Details | Information |
|---|---|
| Project Name | Apex-1 |
| Project By | Omer  |
| Software | EasyEDA Pro |
| Development Time | 13 Hours |
| Microcontroller | STM32F103RBT7 |

## About the Project

I started by designing the complete circuit schematic in EasyEDA Pro. I first integrated the STM32 microcontroller and worked on its supporting circuitry, including decoupling capacitors, voltage connections, boot buttons and switches.

After that, I developed the power management section using voltage regulators and buck-converter circuitry. I then added the line-following sensor interfaces, supporting resistors and connections to the microcontroller. Finally, I integrated the motor driver, battery input, motor connectors and other power-related components to bring all the major electronic sections together.

## Making the Design Beginner-Friendly

During my first design review, I realised that almost all the components I had selected were SMD. Although SMD components are great for compact designs, I wanted Apex-1 to be something beginners could also assemble and understand.

So I went back to the schematic and redesigned the component selection. I replaced suitable SMD resistors and capacitors with through-hole alternatives, revisited the microcontroller and motor driver implementation, and checked the sensor circuitry, LEDs and supporting components. The goal was to make the PCB easier to solder, inspect and repair without compromising the intended functionality.

## PCB Design

Once the revised schematic was ready, I moved on to the PCB layout. I wanted the board to reflect the Formula 1 inspiration, so I spent time working on its overall shape and refining the outline instead of simply going with a standard rectangular PCB.

After establishing the board shape, I arranged the microcontroller, power management, sensor and motor driver sections. I then started routing the connections, paying attention to power distribution, signal connections and the placement of external connectors.


After routing, I reviewed the overall layout and checked the component placement and connections against the schematic.

## What I Learned

This project helped me understand that PCB design is about much more than connecting components. I learned to think about component accessibility, power distribution, circuit organisation and how a schematic translates into an actual physical board.

One of my biggest takeaways was that a technically functional design should also be practical for someone else to build. That is what motivated me to revisit the original SMD-heavy design and make Apex-1 more beginner-friendly.
<img width="3332" height="2362" alt="SCH_Schematic1_2-SENSORS_2026-11-08" src="https://github.com/user-attachments/assets/ea81d6df-6b83-4533-95d6-7ce9e9e7628f" />
<img width="3332" height="2362" alt="SCH_Schematic1_1-POWER_2026-11-08" src="https://github.com/user-attachments/assets/c18323f0-2bc9-4d35-bdcd-b4e78f6603cd" />
