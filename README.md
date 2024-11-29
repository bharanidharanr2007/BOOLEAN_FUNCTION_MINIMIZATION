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

Developed by: RegisterNumber:24900848
```
module exp2(a,b,c,d,x,y,z,w,f1,f2);
input a,b,c,d,x,y,z,w;
output f1,f2;
assign f1=~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2=x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule 
```
**RTL realization**
![alt text](<Screenshot 2024-11-29 110602.png>) 
**truth table**
![alt text](<WhatsApp Image 2024-11-29 at 11.09.27_86decacd.jpg>)

**RTL**
![alt text](<Screenshot 2024-11-29 110302.png>)
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

