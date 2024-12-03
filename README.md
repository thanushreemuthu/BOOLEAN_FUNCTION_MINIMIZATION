# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions.

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Thanushree M RegisterNumber:24900590

```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
*/


**RTL realization**
BOOLEAN FUNCTION MINIMIZATION

F1
![Screenshot 2024-11-20 153945](https://github.com/user-attachments/assets/6f0b2937-bd5e-4fd8-80e2-6aed5adbc58d)

F2
![Screenshot 2024-11-20 154856](https://github.com/user-attachments/assets/044769a7-595b-4cd8-9916-a8cafbf4d190)


**Timing Diagram**
BOOLEAN FUNCTION MINIMIZATION

F1
![Screenshot 2024-11-20 154323](https://github.com/user-attachments/assets/aaafaf3f-06b3-4051-95a9-c63f89ab8f95)

F2
![Screenshot 2024-11-20 155058](https://github.com/user-attachments/assets/206800fd-81fb-40f5-bec6-d47cec546ca3)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

