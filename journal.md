# APEX-1
### F1-Inspired High-Speed Line-Following Robot
## Hours worked *12hour*
APEX-1 is a custom-designed, high-speed line-following robot inspired by Formula 1 racing cars. The project focuses on developing a dedicated PCB that brings together the microcontroller, power management, sensor interfaces and motor control circuitry into one integrated platform.

I wanted to build something beyond a conventional line-following robot. My goal was to design the electronics myself, understand how each section works and create a PCB that is not only functional but also approachable for people who are new to hardware development.


## 15th of September 2026

Started working on the electronics for APEX-1 in EasyEDA Pro. I wanted to design a custom PCB around the STM32F103RBT7 instead of using separate development boards and modules.

I began with the main microcontroller circuit. Added its power and ground connections, decoupling capacitors, boot button and supporting circuitry. I also started planning the connections for the sensors, motor driver and other peripherals.

After that, I worked on the power management section. Added the battery input, voltage regulation and buck converter circuitry to provide the required power to the different sections of the board.

I then started developing the line-following sensor interfaces, including their signal connections and supporting resistors. I also worked on the motor driver section, adding the connections for controlling two DC motors.

**Issue I faced:** During the initial design, I realised that most of my selected components were SMD. This could make the board difficult for beginners to assemble, especially without proper soldering equipment. I decided to revisit the component selection before moving further with the PCB.

<img width="1593" height="648" alt="Screenshot 2026-11-13 115317" src="https://github.com/user-attachments/assets/ac841a2c-a310-4a63-9257-08f1f3f405a8" />
<img width="1487" height="652" alt="Screenshot 2026-11-13 115331" src="https://github.com/user-attachments/assets/e0f4e3d0-7401-4231-b6ae-5b8d5a7153ce" />


**Total time spent: 2 hours**

---

## 15th of September 2026

Spent more time reviewing the schematic and making changes to the original component selection.

I went through the different sections and started identifying components that could be replaced with through-hole alternatives. I focused mainly on resistors, capacitors, LEDs and suitable supporting components used in the sensor and control circuits.

I also revisited the STM32 and motor driver sections to review their connections and component arrangements. The idea was to make the board easier to solder, inspect and repair without changing the intended functionality.

After making the changes, I checked the power connections, sensor signals, motor outputs, switches and supporting circuitry again.

**Issue I faced:** Finding suitable through-hole alternatives was not always straightforward. I had to consider component availability, package dimensions and whether the replacement would work with the existing circuit.

<img width="1907" height="817" alt="Screenshot 2026-11-13 134846" src="https://github.com/user-attachments/assets/bcff613b-50e7-459b-b947-39af7e983098" />
<img width="1915" height="851" alt="Screenshot 2026-11-13 134829" src="https://github.com/user-attachments/assets/24326d23-ddc3-4800-ae6c-6b0269511f12" />


**Total time spent: 2 hours**

---

## 4th of October 2026

Started working on the actual PCB layout in EasyEDA Pro.

Since APEX-1 is inspired by Formula 1 cars, I didn't want to go with a standard rectangular PCB. I started experimenting with the board outline to give it an elongated racing-car-inspired shape, with a wider front section.

Once I was happy with the general outline, I started placing the major components. I worked on arranging the STM32, power management circuitry, motor driver and sensor connections within the available space.

I also considered where the external connectors and through-hole components should go so they would remain accessible during assembly.

**Issue I faced:** The custom PCB shape made component placement a little more challenging. I had to keep checking the available space and moving components around to avoid an overcrowded layout.

<img width="1552" height="858" alt="Screenshot 2026-11-08 141423" src="https://github.com/user-attachments/assets/71baeaa3-2037-4baa-8a84-dbf93ce5debf" />


**Total time spent: 2 hours**

---

## 4th of October 2026

Continued working on the PCB layout, mainly focusing on routing.

I started connecting the components according to the schematic, working through the microcontroller, power management, sensor and motor driver sections.

I also routed the battery input, motor outputs and other external connections. While routing, I tried to keep the power and signal connections organised and make the overall layout easier to follow.

After completing the main routing, I went back through the board and reviewed the component positions and connections against the schematic.

**Issue I faced:** Routing around the custom board outline while keeping the connections organised took some adjustment. I had to revisit a few component positions and routing paths to make better use of the available space.
<img width="1870" height="797" alt="Screenshot 2026-11-13 135119" src="https://github.com/user-attachments/assets/24d718b6-0659-4567-a810-a58e44c88550" />
<img width="1875" height="800" alt="Screenshot 2026-11-13 135130" src="https://github.com/user-attachments/assets/9b7dcb9f-4b02-4da6-97cf-951065d63d00" />


**Total time spent: 2 hours**

---

## 4th of October 2026

Spent the final part of this work session reviewing the overall PCB design.

I checked the board outline, component placement, routing and external connectors. I also looked at the 3D PCB view to get a better idea of how the actual board would look once manufactured.

I went back to the schematic and compared the different connections with the PCB layout, particularly the STM32, power section, sensor interfaces and motor driver.

I also checked whether the through-hole component selection was reflected properly in the physical layout.

The main PCB layout was now in place, with the major electronic sections arranged on the custom Formula 1-inspired board.

**Issue I faced:** I needed to make sure that the custom shape didn't compromise component accessibility or the routing. Reviewing the 3D view helped me look at the design from a more physical perspective.
<img width="2160" height="2667" alt="PCB_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/16922c83-be82-4bac-9cde-77b6e7bb999c" />


<img width="1046" height="567" alt="Screenshot 2026-11-08 141439" src="https://github.com/user-attachments/assets/fafbfca5-ef30-4dac-ab9e-e5e2833c88fd" />

<img width="1552" height="858" alt="Screenshot 2026-11-08 141423" src="https://github.com/user-attachments/assets/df41f790-a208-4faa-8aec-5238be7a3b8f" />



**Total time spent: 4 hours**

---



##  What I Learned

APEX ONE helped me understand that PCB development is not just about connecting components and making a circuit work.

One of the biggest lessons was that component selection has a direct impact on how accessible a hardware project can be.

My initial design was mostly SMD-based, but after reviewing it, I realised that I could make the project more approachable by reconsidering the component packages.

I also gained more experience with schematic development, microcontroller integration, power management, sensor interfacing, motor control and PCB routing.

Most importantly, I learned to look at a PCB from both an electrical and a practical perspective.

A good design should not only work as intended but should also be understandable, accessible and maintainable.
<img width="3332" height="2362" alt="SCH_Schematic1_2-SENSORS_2026-11-08" src="https://github.com/user-attachments/assets/69bf76c5-cbdc-4699-ba62-ca44beb0e450" />
<img width="3332" height="2362" alt="SCH_Schematic1_1-POWER_2026-11-08" src="https://github.com/user-attachments/assets/8c60b4bf-8bc2-47c9-be65-165a2fd9bcdd" />
<img width="2160" height="3022" alt="3D_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/9e9a2230-a3a6-4615-af19-3c6595b14094" />

**Software:** EasyEDA Pro

