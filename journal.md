# APEX ONE 
### F1-Inspired High-Speed Line-Following Robot
## Hours worked *13hour*
APEX ONE is a custom-designed, high-speed line-following robot inspired by Formula 1 racing cars. The project focuses on developing a dedicated PCB that brings together the microcontroller, power management, sensor interfaces and motor control circuitry into one integrated platform.

I wanted to build something beyond a conventional line-following robot. My goal was to design the electronics myself, understand how each section works and create a PCB that is not only functional but also approachable for people who are new to hardware development.

An important part of this project was rethinking my initial design. I originally used mostly SMD components, but later decided to redesign several sections using through-hole components wherever practical. This would make the board easier to assemble, solder, inspect and repair, especially for beginners.
<img width="1891" height="871" alt="Screenshot 2026-11-08 141529" src="https://github.com/user-attachments/assets/578088fc-2138-48bc-8351-116090a64d73" />

---

## 1. Initial Schematic Development

I started the project by developing the electronic architecture in EasyEDA Pro.

Before moving towards the PCB layout, I wanted to establish all the major hardware sections and understand how they would communicate with each other.

I divided the circuit into several sections:

- Main microcontroller and supporting circuitry.
- Power management and voltage regulation.
- Line-following sensor interfaces.
- Motor driver and motor connections.
- Battery and power distribution.
- Boot, reset and control switches.
- LEDs and status indicators.

This gave me a clearer understanding of how the complete robot would be structured and helped me develop the schematic in an organised way.

## 2. STM32 Microcontroller Integration
<img width="1536" height="868" alt="Screenshot 2026-11-08 141819" src="https://github.com/user-attachments/assets/0afacb5b-2bde-46f6-a9e7-50024c03bccb" />

The first major component I worked on was the STM32 microcontroller.

I imported the STM32F103RBT7 into the schematic and started building the surrounding circuit.

After adding the MCU, I worked on its supporting connections, including decoupling capacitors, voltage supply connections, ground connections and the required control circuitry.

I also added the boot button and other necessary switches to make the controller more accessible during programming and hardware operation.

Once the basic MCU circuit was established, I started connecting the required signals for the different sections of the robot.

The microcontroller would act as the central processing unit, receiving information from the sensors and providing control signals to the motor driver.

## 3. Power Management and Voltage Regulation

After completing the initial microcontroller section, I moved towards the power management circuitry.

I added the required voltage regulators and buck-converter circuitry to handle the different power requirements of the board.

I also incorporated the supporting components and connections needed for the power regulation section.

The main objective was to establish an organised power distribution system for the microcontroller, sensors and motor control circuitry.

I then connected the power-related sections and reviewed how the different components would receive their required supplies.
<img width="1891" height="871" alt="Screenshot 2026-11-08 141529" src="https://github.com/user-attachments/assets/0d957acf-2ac9-4540-bae3-ab25842938b1" />

## 4. Sensor Circuit Development

The next stage was developing the line-following sensor section.

Since APEX ONE is designed around line-following functionality, I needed to establish the sensor interfaces and connect them to the STM32.

I added the required sensor connections along with the supporting resistors and other necessary components.

I then connected the sensor signals to the appropriate microcontroller pins.

I also reviewed the supporting circuitry to ensure that the sensor section was properly integrated into the overall schematic.
<img width="1046" height="567" alt="Screenshot 2026-11-08 141439" src="https://github.com/user-attachments/assets/fafbfca5-ef30-4dac-ab9e-e5e2833c88fd" />

## 5. Motor Driver and Power Output Section

Once the microcontroller and sensor sections were established, I moved towards the motor control circuitry.

I added the motor driver IC and developed the connections required to control the two DC motors.

This section included the motor driver, motor output connectors, battery connections, supporting components and the required control signals from the STM32.

I also added the necessary power connections and switches.

Since the motors are responsible for the robot's movement, I wanted their circuitry to be properly organised and integrated with the main controller.

At this point, the initial schematic contained the major electronic sections required for the robot.

---

## 6. First Design Review: Making the PCB Beginner-Friendly

After completing the initial schematic, I started reviewing the component selection.

This was when I noticed something I hadn't considered properly during the initial design.

Almost all the components I had selected were SMD components.

Although SMD components are useful for compact PCB designs, they can be difficult for beginners to solder and replace without the right equipment and experience.

I wanted APEX ONE to be a project that someone interested in electronics could actually build and understand.

So, instead of continuing with the original component selection, I decided to revisit the design and make it more beginner-friendly.

This meant reconsidering the component packages and replacing suitable SMD components with through-hole alternatives.

## 7. Component Redesign and Through-Hole Conversion

This was one of the most important stages of the project.

I started going through the components in the schematic and identifying which ones could be changed without affecting the intended functionality of the circuit.

### Microcontroller

I revisited the microcontroller implementation and incorporated the STM32 microcontroller into the revised hardware design, rather than treating the controller section as simply an SMD-based component arrangement.

I also reviewed its supporting connections and accessibility.

### Motor Driver

I revised the motor driver section and incorporated the selected motor driver component into the updated design.

I reviewed its connections and supporting circuitry to ensure that the motor control section remained properly integrated.

### Resistors and Capacitors

I went through the passive components and replaced suitable SMD resistors and capacitors with through-hole alternatives.

This included components used in the sensor circuits and other supporting sections of the board.

The idea was to make commonly handled components easier to identify, solder and replace.

### Sensor Components

I also revisited the sensor-related components and their supporting circuitry.

I reviewed the resistor connections and other components required for the line-following sensor section.

The aim was to make the sensor circuitry more accessible without losing the original functionality.

### LEDs and Indicators

I checked the LED implementation across the board and reviewed the associated components and connections.

I wanted to ensure that the indicator section remained properly integrated into the revised design.

After completing these changes, I went through the component selection again to check that the updated packages and connections were consistent with the schematic.

## 8. Revised Schematic Review

Once the component redesign was complete, I returned to the schematic for another review.

I checked the updated component connections and reviewed the different sections to make sure that the redesign had not introduced inconsistencies.

I particularly focused on:

- STM32 connections.
- Power supply and voltage regulation.
- Buck-converter circuitry.
- Sensor interfaces.
- Motor driver connections.
- Resistor and capacitor replacements.
- Switches and boot controls.
- LED connections.
- Battery and motor connectors.

After reviewing the revised schematic, I moved towards the physical PCB design.

---

## 9. PCB Shape and Layout Development

With the schematic ready, I started working on the actual PCB layout in EasyEDA Pro.

Since APEX ONE is inspired by Formula 1 cars, I wanted the PCB to reflect that concept.

I started thinking about the overall board shape, its dimensions and how the different components would fit within the available space.

This required some planning because the PCB needed to accommodate several different sections while maintaining a clean and practical arrangement.

I considered the placement of the microcontroller, power management components, sensors, motor driver and external connectors.

After working through the overall shape and refining the board outline, I started arranging the components within the PCB.
<img width="1552" height="858" alt="Screenshot 2026-11-08 141423" src="https://github.com/user-attachments/assets/df41f790-a208-4faa-8aec-5238be7a3b8f" />

## 10. Component Placement

Once the board outline was established, I started placing the components.

I worked through the different sections of the PCB and arranged the components according to their functionality and connections.

I focused on keeping the microcontroller section organised, positioning the power management circuitry appropriately and making the motor driver and external connectors accessible.

I also considered the placement of the through-hole components because one of the main objectives of the redesign was to make assembly easier for beginners.

This stage involved reviewing the arrangement multiple times and refining the component positions to achieve a cleaner overall layout.

## 11. PCB Routing

After completing the component placement, I moved towards routing the PCB.

I started connecting the components according to the schematic and worked through the different sections of the board.

The routing process involved connecting the microcontroller, power management circuitry, sensor interfaces and motor driver.

I also worked on the battery input, motor outputs and other external connections.

While routing, I considered the separation of power and signal connections and the physical arrangement of the different circuit sections.

I wanted the final routing to be organised and consistent with the intended circuit architecture.

Once the connections were established, I reviewed the PCB layout and refined the routing where necessary.

## 12. Final PCB Review

After completing the routing, I reviewed the overall PCB design.

I checked the component arrangement, board outline, routing and connections to ensure that everything followed the intended schematic.

I also reviewed the physical accessibility of the components and the overall layout.

The final review focused on making sure that the PCB maintained the original design objectives:

- An integrated STM32-based control system.
- Dedicated power management circuitry.
- Integrated line-following sensor connections.
- Dual-motor control circuitry.
- Beginner-friendly component selection.
- A practical and organised PCB layout.
- An F1-inspired physical design.
<img width="2160" height="2667" alt="PCB_PCB1_2026-11-08" src="https://github.com/user-attachments/assets/16922c83-be82-4bac-9cde-77b6e7bb999c" />

---

## 13. What I Learned

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

