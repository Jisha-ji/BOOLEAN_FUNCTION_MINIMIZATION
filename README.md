# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Software-quartus prime ,cyclone V

**Theory**

 Boolean function minimization is the process of simplifying Boolean
expressions, reducing the number of terms or literals without changing the functionality.
Simplifying Boolean functions is essential for designing efficient digital circuits, as it
reduces the number of gates required, minimizing cost, power consumption, and circuit
complexity.

**logic diagram**


![WhatsApp Image 2024-12-26 at 15 44 23_35f95b30](https://github.com/user-attachments/assets/28e9bbea-55af-46eb-b829-2b8a452fa201)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Jisha Bossne SJ  RegisterNumber: 24900154 */
```
1)module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
2)module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**Output:**

function 1:

![exp2 output2](https://github.com/user-attachments/assets/c805f89d-2704-481f-920e-0e47281d1b8f)

function 2:

![exp-2a f2 last](https://github.com/user-attachments/assets/7f49c916-3688-4460-8a82-2965cf266ccf)


**RTL**

function 1:

![exp-2](https://github.com/user-attachments/assets/b9414595-4345-45ec-8059-363f7e137f83)

function 2:

![exp-2 output2](https://github.com/user-attachments/assets/abeff791-0d27-45d4-b9e1-3324cd9c9906)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

