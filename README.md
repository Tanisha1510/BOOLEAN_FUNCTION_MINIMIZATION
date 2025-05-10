# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions.

![image](https://github.com/user-attachments/assets/ef2bc123-f178-45c2-a1f5-05a34f907720)
F1 
![image](https://github.com/user-attachments/assets/049bc341-112f-46ab-b0d2-8c7cef84dd83)
F2
![image](https://github.com/user-attachments/assets/cfaeadc1-b4fd-479d-bb1b-a25e91e1e250)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
F1
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

F2
```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
Developed by: Tanisha S RegisterNumber:212224050053*/


**RTL realization**
F1
![image](https://github.com/user-attachments/assets/5345d311-4ede-4514-ba98-1f83f43dd026)
F2
![image](https://github.com/user-attachments/assets/32921038-bbac-45cd-8509-fa17611be10b)


**Timing Diagram**
F1
![image](https://github.com/user-attachments/assets/b4a1fb52-0ce3-4844-8adc-a0474f8784d6)
F2
![image](https://github.com/user-attachments/assets/925dfceb-7669-46e9-9508-1a8054fe7ca8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

