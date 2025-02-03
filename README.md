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

Developed by: RegisterNumber:*/24901213
```
module de2(a,b,c,d,f1);

input a,b,c,d;
output f1;
assign f1=  (~b&~d) | (a&b&~c) | (~a&b&d);
endmodule
2.module de2_2(w,x,y,z,f2);

input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
**RTL realization**

1.![alt text](<Screenshot 2024-11-26 115128.png>)

2.![alt text](<Screenshot 2024-11-26 113958.png>)

**Output:**

**RTL**

**Timing Diagram**
1.![alt text](<Screenshot 2024-11-26 111904.png>)

2.![alt text](<Screenshot 2024-11-26 114504.png>)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

