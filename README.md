### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![WhatsApp Image 2025-10-15 at 10 06 03_cb3f1497](https://github.com/user-attachments/assets/34b1da71-630c-401f-9ce9-3c66a76f0eda)


Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**
<img width="1911" height="826" alt="image" src="https://github.com/user-attachments/assets/ec73d01c-35d0-4c95-b177-d9a950000572" />

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:DWIJESH RAJ SINHA Y RegisterNumber:25013468
*/

**RTL LOGIC UP COUNTER**
![WhatsApp Image 2025-10-15 at 10 05 56_c76d9bd1](https://github.com/user-attachments/assets/7f82a927-d2d4-47b9-a702-1b2f612f6e22)

**TIMING DIAGRAM FOR IP COUNTER**

**TRUTH TABLE**

**RESULTS**
