# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**
software-quartus prime, cyclone V

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean expressions, reducing the number of terms or literals without changing the functionality. Simplifying Boolean functions is essential for designing efficient digital circuits, as it reduces the number of gates required, minimizing cost, power consumption, and circuit complexity.

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Jisha Bossne SJ  RegisterNumber:24900154
'''
1)module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

2)module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule'''

**Output:**
![exp2 output2](https://github.com/user-attachments/assets/8fc3732e-06b3-45e8-95a7-743e279a4345)

![exp-2a f2 last](https://github.com/user-attachments/assets/ef2f6640-1052-4fff-8589-cf3890a519db)

**RTL**
![exp2 output2](https://github.com/user-attachments/assets/71a8b867-4425-4095-be76-bb1e825b5d6f)

![exp-2a f2 last](https://github.com/user-attachments/assets/ea25668e-4abe-4b9a-b75b-8593cb2a1f4a)


**Timing Diagram**
![exp-2](https://github.com/user-attachments/assets/3b77617a-5a66-4db2-9500-f596b2c30c87)

![exp-2 output2](https://github.com/user-attachments/assets/72f969ea-b3a6-4e56-be4f-89aea3faab3c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

