### SYNCHRONOUS-UP-COUNTER

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
1.Initialize the shift register to a known state (e.g., all zeros).<br>

2.Input a bit serially into the shift register.<br>

3.Shift the contents of the register one position to the right (or left).<br>

4.Output the shifted bit from the last stage of the register.<br>

5.Repeat steps 2-4 for each bit you want to input and shift.<br>



**PROGRAM**
<br>

 Program for flipflops and verify its truth table in quartus using Verilog programming. <br>

Developed by:S.Suriya prakash<br>
RegisterNumber:212223100055
```
module ex10(clk, sin, q);
input clk;
input sin;
output [3:0] q;
reg [3:0] q;
always @(posedge clk)
begin
q[0] <= sin;
q[1] <= q[0];
q[2] <= q[1];
q[3] <= q[2];
end
endmodule
```


**RTL LOGIC UP COUNTER**<br>

![image](https://github.com/arulsuriyalokeshy/SYNCHRONOUS-UP-COUNTER/assets/149130151/37028e57-e5f1-4df8-9924-6cc3e66467a0)


**TIMING DIAGRAM FOR IP COUNTER**<br>

![image](https://github.com/arulsuriyalokeshy/SYNCHRONOUS-UP-COUNTER/assets/149130151/723dbb95-63e2-42fb-9b67-4298d2d4758d)


**TRUTH TABLE**<br>
![image](https://github.com/arulsuriyalokeshy/SYNCHRONOUS-UP-COUNTER/assets/149130151/1d64dc88-3ebb-418c-a2fa-2a7cfd41d2a7)


**RESULTS**<br>
SISO Shift Register using verilog and validating their functionality using their functional tables has successful execution of the program.
