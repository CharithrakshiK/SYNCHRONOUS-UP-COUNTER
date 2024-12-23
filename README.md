# EXP:11: SYNCHRONOUS UP COUNTER
# NAME: CHARITHRAKSHI K
# REG.NO: 24900651

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**



**PROGRAM**

![WhatsApp Image 2024-12-23 at 11 44 21_73ade680](https://github.com/user-attachments/assets/60b6631c-a601-4e7b-8674-195cb415e6fa)


**RTL LOGIC UP COUNTER**

![{670FCE3B-DCBB-4FE1-B007-5FDB43FF3875}](https://github.com/user-attachments/assets/b6919aa6-b437-42eb-82dc-4f6bc2fdaf99)


**TIMING DIAGRAM FOR IP COUNTER**

![WhatsApp Image 2024-12-23 at 11 44 22_e4f12d0d](https://github.com/user-attachments/assets/f6040540-35a3-4117-af47-6c0d735a7d42)


**TRUTH TABLE**

![WhatsApp Image 2024-12-23 at 11 36 47_d1a9fda5](https://github.com/user-attachments/assets/3d058ead-0617-40e6-b7de-61ca9ab47bd3)


**RESULTS**

THUS THE SYNCHRONOUS UP COUNTER IS STUDIED AND EXECUTED SUCCESSFULLY 
