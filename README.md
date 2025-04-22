PCB Design Portfolio
___________________________________________________________________________________________________________
My name is Matthew Gorbold McCardle, and I am an electrical engineering student set to graduate in May 2026. This repository serves as a portfolio of my PCB design work using Altium. To date, I have designed four boards, progressing from foundational test designs to complex, practical applications. All Altium design files are included in this repository for review. Feel free to reach out to me on LinkedIn: www.linkedin.com/in/matthewgorboldmccardle
___________________________________________________________________________________________________________
Table of Contents
___________________________________________________________________________________________________________
Board 1: LED Dimming Test Board (#board-1-led-dimming-test-board)  

Board 2: Grounding Techniques Comparison (#board-2-grounding-techniques-comparison)  

Board 3: Custom Arduino Design (#board-3-custom-arduino-design)  

Board 4: Power Source Integrity Measurement Device (#board-4-power-source-integrity-measurement-device)  

Skills Demonstrated

About Me

___________________________________________________________________________________________________________
Board 1: 
The goal of this first board design is to first practice and develop Altium and PCB design experience, and second to measure the effectiveness of dimming LEDs using different strength resistors. The initial design concept for the board is shown below:
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/e8412671-85f8-45cc-9325-c8c83f7fa738)
___________________________________________________________________________________________________________
Schematic design for board 1.

___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/6cf29fb6-8279-40fe-a962-a08cacec4a1a)
___________________________________________________________________________________________________________
Final board layout for board 1.
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/08935a35-f25e-4fce-b376-729195c34837)
___________________________________________________________________________________________________________
Assembled board 1 with 5V power and both switches on.
___________________________________________________________________________________________________________
The design works as intended, the 555 timer provides a pulse signal to the LEDs, and the brightness of each LED increases as the resistance of each resistor decreases. In the measurement of the voltage across the 1k Ohm resistor we see minimal switching noise.
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/41215f39-b0d2-4993-9770-3a55c78191be)
___________________________________________________________________________________________________________
Board 2: 
The goal of my second board is to test the differences in grounding methods between using no ground planes and a close decoupling capacitor versus proper use of the ground plane and location of decoupling capacitor. I designed 2 hex inverter circuits, one using good grounding techniques with vias, a ground plane and decoupling capacitors located close to power inputs and the other using poor practices, using no ground plane, connecting all grounds by wire, and distant decoupling capacitors.
![image](https://github.com/user-attachments/assets/63ffeb75-c8ce-4964-afdf-6c8bfd78aad2)
___________________________________________________________________________________________________________
Schematic design for board 2.
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/0dee3c17-3753-4219-bdc7-94463b1dc234)
___________________________________________________________________________________________________________
Final board layout for board 2.
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/eb67a606-3b03-44b7-a345-ce86c645f7bf)
___________________________________________________________________________________________________________
Assembled board 2 with power connected.
___________________________________________________________________________________________________________
The bad practices hex inverter had drastically more noise than the good one as expected. I saw an average of 50% reduction in switching noise across measured 8 metrics.
___________________________________________________________________________________________________________

Board 3: 
The goal of my third board project is to create my own Arduino that is better than a commercial Arduino.
___________________________________________________________________________________________________________
![Screenshot 2025-04-04 173743](https://github.com/user-attachments/assets/4f8d477a-bbeb-4c0d-a2a0-1583edaf6809)
___________________________________________________________________________________________________________
Schematic design for board 3.
___________________________________________________________________________________________________________
![Screenshot 2025-04-04 174552](https://github.com/user-attachments/assets/75d5f4c3-a66d-4e29-9eea-86b4dccb4847)
___________________________________________________________________________________________________________
Final board layout for board 3.
___________________________________________________________________________________________________________
After completing this design I found that I could improve it by better placing my decoupling capacitors C12 and C13 to better filter power line noise. I found my board produces 22% less amplitude of switching noise, but this could be improved further. 
___________________________________________________________________________________________________________
Board 4:
The goal of my fourth board is to create an instrument drone to measure the integrity of power sources. The device measures and calculates the thevenin voltage and resistance of power sources. This board is a four layer, double sided board, the middle two layers are both grounded, the back side is an Arduino, and the front side has the power management circuits, with smart LEDs and a buzzer.
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/8552e86a-ed5f-4092-bec8-42b3baea5006)
___________________________________________________________________________________________________________
Schematic design for board 4
___________________________________________________________________________________________________________
![image](https://github.com/user-attachments/assets/d38b19a8-76b8-4806-94b3-d9bdbf4f0f24)
___________________________________________________________________________________________________________
Final front board layout for board 4.
___________________________________________________________________________________________________________

![image](https://github.com/user-attachments/assets/25bb8ba6-d0fe-4d70-bb7d-13259934b4d4)
___________________________________________________________________________________________________________
Final back board layout for board 4.
___________________________________________________________________________________________________________
I am in the process of building this board, so no analysis has been done yet.
___________________________________________________________________________________________________________
Skills Demonstrated: 
___________________________________________________________________________________________________________
PCB Design with Altium: Proficient in creating schematics and layouts.  

Signal Integrity: Applied techniques to minimize noise and ensure reliable operation.  

Grounding Techniques: Demonstrated effective use of ground planes and vias.  

Component Selection and Placement: Optimized designs for performance.  

Multi-Layer Board Design: Managed complex layouts with grounded layers.  

Testing and Measurement: Quantified improvements through empirical data.
___________________________________________________________________________________________________________
About Me: 
___________________________________________________________________________________________________________
Through these projects, I have built a solid foundation in PCB design, focusing on signal integrity, grounding, and practical applications. My work reflects a progression from learning fundamentals to tackling sophisticated designs, such as multi-layer boards and custom microcontrollers. I am eager to apply these skills in a professional environment, contributing to innovative engineering solutions while continuing to refine my expertise.


