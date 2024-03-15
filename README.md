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


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Jeshwanth Kumar
RegisterNumber: 212223240114
*/


**RTL realization**
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

**Output:**
![image](https://github.com/Jeshwanthkumarpayyavula/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742402/157dae71-cf10-48c6-8822-33130c374df2)
![image](https://github.com/Jeshwanthkumarpayyavula/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742402/2825648a-1a53-48f9-8ec3-8fc4c6924d19)


**RTL**


**Timing Diagram**
![image](https://github.com/Jeshwanthkumarpayyavula/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742402/f6d50df2-f069-4880-b2f3-5451ae6eb75b)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

