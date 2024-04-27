# EX02 BOOLEAN_FUNCTION_MINIMIZATION

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

Developed by: Aditaayan m
RegisterNumber: 212223040006 */
``` 
module booleanfunction(A,B,C,D,F1); 
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
```
![316327265-678658cf-4682-484c-a8af-3b3083fbd22a](https://github.com/Aditaayan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473394/0af426c0-a0bf-43c0-a4c4-828fcb18e5e1)


**RTL realization**

![316327275-69e72eb5-88c2-4e05-8069-1890417e261c](https://github.com/Aditaayan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473394/a527341a-95c6-4192-b655-fa28e4c36811)




**Output:**

![316327286-79278d5e-3b0c-4a4a-9430-a2d49b7d385e](https://github.com/Aditaayan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473394/384344ad-76c8-4ca1-b7cd-717de6910ba1)






**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

