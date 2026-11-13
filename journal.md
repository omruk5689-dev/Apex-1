# APEX-1
### F1-Inspired High-Speed Line-Following Robot
## Hours worked *12hour*
APEX-1 is a custom-designed, high-speed line-following robot inspired by Formula 1 racing cars. The project focuses on developing a dedicated PCB that brings together the microcontroller, power management, sensor interfaces and motor control circuitry into one integrated platform.

I wanted to build something beyond a conventional line-following robot. My goal was to design the electronics myself, understand how each section works and create a PCB that is not only functional but also approachable for people who are new to hardware development.
# APEX-1
### F1-Inspired High-Speed Line-Following Robot

**Total Hours Worked: 12 Hours**

APEX-1 is a custom-designed, Formula 1-inspired line-following robot. The main idea behind this project is to develop a dedicated PCB that brings the robot's major electronics together on a single board, including the STM32 microcontroller, power management, sensor interfaces and motor control.

I wanted to build something beyond a conventional line-following robot. Instead of using separate development boards and modules, I wanted to design the electronics myself and understand how everything fits together.

One thing I also wanted to focus on was making the design beginner-friendly. My initial component selection was mostly SMD-based, but after reviewing it, I decided to replace suitable components with through-hole alternatives wherever practical. This would make the board easier to solder, inspect and repair.



---

## 1. Initial Schematic Development
**Date:** September 15, 2026  
**Time Worked:** 1 Hour

I started by planning the complete electronic architecture in EasyEDA Pro. Before getting into the PCB layout, I wanted to make sure I had all the major sections figured out.

I divided the design into different sections:

- Main microcontroller and supporting circuitry.
- Power management and voltage regulation.
- Line-following sensor interfaces.
- Motor driver and motor connections.
- Battery input and power distribution.
- Boot, reset and control switches.
- LEDs and status indicators.

This gave me a basic structure to work with and helped me understand how all the different sections would connect.

### STM32 Microcontroller Integration

The first major part of the schematic was the STM32F103RBT7.

I added the microcontroller and started working on its supporting circuitry, including decoupling capacitors, power connections, ground connections and control signals.

I also included the boot button and switches needed for programming and basic hardware control.

The STM32 would be the main controller of APEX-1, handling sensor inputs and sending the necessary signals to the motor driver.
<img width="1593" height="648" alt="Screenshot 2026-11-13 115317" src="https://github.com/user-attachments/assets/647e9065-2c4a-4487-91af-66d1d2e1981c" />


### Power Management

I also started planning the power section, including the buck converter, voltage regulation and battery input.

Since the board contains several different electronic sections, I wanted to keep the power distribution organised and provide the required supply voltages to the controller and peripherals.

---

## 2. Sensor Circuit Development
**Date:** September 15, 2026  
**Time Worked:** 1 Hour

Next, I worked on the line-following sensor interfaces.

Since the main purpose of APEX-1 is to follow a track, the sensor section is one of the most important parts of the design.

I added the sensor connections and their supporting resistors, then connected the signal lines to the STM32.

I also reviewed the connections to make sure the sensor section would fit properly into the overall circuit.



<img width="1487" height="652" alt="Screenshot 2026-11-13 115331" src="https://github.com/user-attachments/assets/ce591373-d107-4330-bbfe-24a6939e1868" />

After the sensor section, I moved on to the motor control circuitry.

I added the motor driver IC, along with the connections for controlling two DC motors. This section also included the motor output connectors, battery connections and supporting components.

I wanted the motor control section to be properly integrated with the STM32 rather than relying on a separate motor driver module.

By this point, the schematic had the main electronic sections needed for the robot.

---

## 3. First Design Review: Making It Beginner-Friendly
**Date:** September 15, 2026  
**Time Worked:** 2 Hours

After getting the initial schematic together, I went back and reviewed my component selection.

That's when I noticed that almost everything I had selected was SMD.

SMD components are great for compact designs, but they can be a little difficult for someone just getting started with soldering and PCB assembly.

I didn't really want APEX-1 to become a project that only people with specialised soldering equipment could assemble.

So I decided to revisit the design and see which components I could replace with through-hole alternatives without changing the intended functionality.

This meant going through the schematic again and reconsidering the component packages rather than simply continuing with the original design.

---

## 4. Component Redesign and Through-Hole Conversion
**Date:** September 15, 2026  
**Time Worked:** 3.5 Hours

This took longer than I initially expected because I had to review the different sections individually.

I started with the passive components, replacing suitable SMD resistors and capacitors with through-hole versions.

I also revisited the microcontroller, motor driver and sensor sections to check their component selections and supporting circuitry.

### Resistors and Capacitors

I went through the resistors and capacitors used across the different sections and looked for suitable through-hole alternatives.

The main idea was to make commonly handled components easier to solder and replace.

### Microcontroller and Motor Driver

I reviewed the STM32 and motor driver sections, including their supporting connections and component arrangements.

I wanted to keep the main control circuitry organised while making the overall design more practical to assemble.

### Sensor Components and LEDs

I also revisited the sensor circuitry, supporting resistors and LED indicators.

I checked which components could be changed to through-hole packages while keeping the intended connections and functionality.
<img width="1891" height="871" alt="Screenshot 2026-11-08 141529" src="https://github.com/user-attachments/assets/578088fc-2138-48bc-8351-116090a64d73" />

### Revised Schematic Review

After making the changes, I went through the schematic again.

I checked the power connections, sensor interfaces, motor driver signals, switches, LEDs and the different supporting components.

I wanted to make sure that the component changes hadn't introduced any inconsistencies.

Once I was satisfied with the revised schematic, I moved on to the PCB layout.

---

## 5. PCB Shape and Layout Development
**Date:** October 4, 2026  
**Time Worked:** 4 Hours

This was probably the most visually interesting part of the project.

Since APEX-1 is inspired by Formula 1 cars, I didn't want to use a regular rectangular PCB. I wanted the board itself to reflect the design of an F1 car.

I started working on the PCB outline in EasyEDA Pro, experimenting with the overall shape and how the different sections could fit inside it.

The board has an elongated body with a wider front-wing-inspired section, giving it a more racing-inspired appearance.

Of course, getting the shape right wasn't just about appearance. I also had to consider the available space for the microcontroller, power circuitry, motor driver and external connections.
<img width="2160" height="2667" alt="PCB_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/16922c83-be82-4bac-9cde-77b6e7bb999c" />






<img width="1046" height="567" alt="Screenshot 2026-11-08 141439" src="https://github.com/user-attachments/assets/fafbfca5-ef30-4dac-ab9e-e5e2833c88fd" />

<img width="1552" height="858" alt="Screenshot 2026-11-08 141423" src="https://github.com/user-attachments/assets/df41f790-a208-4faa-8aec-5238be7a3b8f" />







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

