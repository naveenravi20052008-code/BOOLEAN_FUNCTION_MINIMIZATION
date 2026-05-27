# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Theory**
Implementing Boolean functions in Verilog HDL (Hardware Description Language) involves translating the simplified Boolean expressions into Verilog code to describe the behavior of digital circuits. The basic building blocks in Verilog is module. The module represent a combinational circuit. Use logical operators (&, |, ~, ^) to implement Boolean functions directly. Use built-in gate primitives for basic functions. Use University program VWF to verify the functionality of your Verilog modules. Create waveform and check outputs against expected results.

**Logic Diagram**
Truth Table for F1
A	B	C	D	F1
0	0	0	0	1
0	0	0	1	0
0	0	1	0	1
0	0	1	1	0
0	1	0	0	0
0	1	0	1	1
0	1	1	0	0
0	1	1	1	1
1	0	0	0	1
1	0	0	1	0
1	0	1	0	1
1	0	1	1	0
1	1	0	0	1
1	1	0	1	1
1	1	1	0	0
1	1	1	1	0
Truth Table for F2
W	X	Y	Z	F2
0	0	0	0	0
0	0	0	1	1
0	0	1	0	0
0	0	1	1	0
0	1	0	0	0
0	1	0	1	1
0	1	1	0	1
0	1	1	1	1
1	0	0	0	0
1	0	0	1	1
1	0	1	0	1
1	0	1	1	1
1	1	0	0	0
1	1	0	1	1
1	1	1	0	1
1	1	1	1	1
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

Developed by: Naveen R
RegisterNumber:212225040276

**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
module Boolean(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|(w & y)|(x & y));
endmodule

**RTL realization**
<img width="1329" height="751" alt="{89C1FB53-C308-4A6D-9B37-36C45A1C0AD5}" src="https://github.com/user-attachments/assets/ef8781c1-ade4-4a8e-99e3-26a2178151c0" />

**Output:**
<img width="1329" height="751" alt="Screenshot 2026-05-27 155242" src="https://github.com/user-attachments/assets/822130ab-47e3-4cc8-a622-9e511363c982" />


**Timing Diagram**
<img width="1293" height="375" alt="Screenshot 2026-05-27 153431" src="https://github.com/user-attachments/assets/ea2ca511-63dc-446d-a36d-f6b6ce9fb34e" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

