This repository is a portfolio of all of my PCB design using Altium, I so far have designed four boards.
The first two boards were test boarding for learning how to use Altium and the importance of signal intergrity in PCB design. The second two were complex designs with applicable use cases. I have attached all Altium design files in the respository.
___________________________________________________________________________________________________________
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
