# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions
**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/24001722

module exp2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

module exp2b(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule

**RTL **
exp2
![Screenshot (1)](https://github.com/user-attachments/assets/00170547-0fda-47d0-94f5-44e3c373184b)


**RTL:**
exp2b
![Screenshot (3)](https://github.com/user-attachments/assets/b2e14044-c94c-472b-853e-66d88e978898)

**Timing diagram**
exp2
![Screenshot (2)](https://github.com/user-attachments/assets/21a48d9d-da8b-4b51-b804-73f5b8eed1b8)

exp2b

![Screenshot (4)](https://github.com/user-attachments/assets/cf58223a-516d-4942-8531-131863bb78d2)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

