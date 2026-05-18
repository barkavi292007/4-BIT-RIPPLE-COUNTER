# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
module digital4(a,b,c,x,y,z,sum,dif,car,bor);
input a,b,c,x,y,z;
output sum,dif,car,bor;
assign sum = a^b^c;
assign car = a&b | a&c | b&c;
assign dif = x^y^z;
assign bor = ~x&z | ~x&y | y&z;
endmodule

```
 Developed by:BHARGAVI S
 RegisterNumber:212225230033

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="1249" height="655" alt="Screenshot 2026-05-18 200159" src="https://github.com/user-attachments/assets/94d10044-ee8e-4f89-9c01-e7fbfdf9664c" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1275" height="677" alt="Screenshot 2026-05-18 200250" src="https://github.com/user-attachments/assets/77f4b423-81cc-482a-8997-9f960b28f6c1" />


**RESULTS**
Thus, To implement 4 Bit Ripple Counter using verilog and validating their functionaly using their functional tables is executed succsessfully.
