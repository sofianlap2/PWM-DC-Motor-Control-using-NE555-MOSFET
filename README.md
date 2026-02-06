# PWM-DC-Motor-Control-using-NE555-MOSFET
PWM DC Motor Control using NE555 &amp; MOSFET

<img width="1017" height="668" alt="image" src="https://github.com/user-attachments/assets/d9105470-6fb7-4ab5-9006-838dc1ac6cc6" />

<img width="1017" height="572" alt="image" src="https://github.com/user-attachments/assets/14d67813-63c4-4d02-bd3b-2da0536afa72" />

<img width="604" height="340" alt="image" src="https://github.com/user-attachments/assets/bace702a-6bd2-4442-8944-4c345a7401ed" />

Project Objective 
The objective of this project is to control the speed of a DC motor using Pulse Width Modulation (PWM). An NE555 timer is used to generate a variable-duty-cycle PWM signal, which drives a power MOSFET. This approach allows efficient speed control with minimal power loss.

Why PWM Instead of Linear Control?
In linear control, a transistor operates in its active region and behaves like a variable resistor.
This causes significant power dissipation as heat (P = V × I), reducing efficiency and requiring
heat sinks. PWM avoids this problem by switching the transistor fully ON or fully OFF, drastically reducing power loss.
1 • High efficiency (low heat dissipation)
2 • Better battery life
3 • Suitable for high-current loads like motors

Duty Cycle and Motor Speed
The duty cycle represents the percentage of time the signal is HIGH during one period. A higher duty cycle increases the average voltage applied to the motor, increasing speed. A lower duty cycle reduces the average voltage, slowing the motor down.

<img width="945" height="490" alt="image" src="https://github.com/user-attachments/assets/6098750d-b205-4488-b446-afb6f2227198" />

 
A logic-level N-channel MOSFET is used as a low-side switch. It can handle high current with very low ON resistance, minimizing conduction losses. A flyback diode is placed across the motor to protect the MOSFET from voltage spikes.
Why MOSFET and not BJT for power control?
MOSFET are preferred for power control over BJT primarily due to their voltage-controlled nature, higher switching speeds, lower power consumption, and improved efficiency. Unlike current-driven BJTs that require constant base current, MOSFETs only need a gate voltage to switch, reducing drive circuit complexity and heat. They also offer lower on-resistance and faster switching speeds.
What I Learned
 1 • Practical PWM generation using NE555 
2 • Duty cycle vs frequency behavior 
3 • Why MOSFETs are preferred for power control 
4 • How PWM improves efficiency in motor control 
This project helped me understand real-world power electronics concepts and reinforced why PWM is the standard technique for efficient motor speed control




