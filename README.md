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

Developed by:Amirthavarshini.R.D

RegisterNumber: 212223040013

module Booleanexpressionmin(a,b,c,d,w,x,y,z,f1,f2); 
input a,b,c,d,w,x,y,z; 
output f1,f2; 
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u; 
not(adash,a); 
not(bdash,b); 
not(cdash,c); 
not(ddash,d); 
not(ydash,y); 
and(p,bdash,ddash); 
and(q,adash,b,d); 
and(r,a,b,cdash); 
or(f1,p,q,r); 
and(s,ydash,z); 
and(t,x,y); 
and(u,w,y); 
or(f2,s,t,u); 
endmodule





**Output:**

![Screenshot 2024-04-02 144328](https://github.com/amirtha5591/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742831/231e3974-a759-441d-b74f-956188c25ad4)




**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.



