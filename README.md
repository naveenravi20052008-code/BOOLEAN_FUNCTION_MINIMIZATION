# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

Developed by:Naveen R
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
<img width="976" height="783" alt="Screenshot 2026-05-27 152303" src="https://github.com/user-attachments/assets/468c8c57-c726-4147-a64d-1fc1a37e087f" />

**Output:**
<img width="1329" height="751" alt="Screenshot 2026-05-27 155242" src="https://github.com/user-attachments/assets/b0e2c874-cd3c-4bc2-b87b-87df2bd1fd71" />

**Timing Diagram**
<img width="1293" height="335" alt="Screenshot 2026-05-27 153431(1)" src="https://github.com/user-attachments/assets/08a15f5e-3ca8-48ab-9e85-c702294af7a1" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


