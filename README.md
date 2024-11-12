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
![LOGIC DIAGRAM EXP-1-1](https://github.com/user-attachments/assets/7762c386-7742-4d9b-be22-dde71bf0d9fd)

![LOGIC DIAGRAM 2-2](https://github.com/user-attachments/assets/77e4a106-931a-444a-989b-396d7ecfc777)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module function1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module function2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Kesavan S 
RegisterNumber: 24003333 */


**RTL realization**

**Output:**

**RTL**
![RTL EXP 2-1](https://github.com/user-attachments/assets/2fefefee-9556-4449-9416-90439108e73c)

![RTL 2-2](https://github.com/user-attachments/assets/32ac5b92-a6f5-4642-a9c0-baa2ae53381c)


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

