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

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

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

**Output:**

**RTL**

Boolean function minimization f1
![Screenshot 2024-11-20 153945](https://github.com/user-attachments/assets/fe01d718-b5e9-4c2a-b506-8aea7d2f07b0)

Boolean function minimization f2
![Screenshot 2024-11-20 154856](https://github.com/user-attachments/assets/fb3f6222-c330-44e1-b834-62d1f1c50e46)

**Timing Diagram**

Boolean function minimization f1
![Screenshot 2024-11-20 154323](https://github.com/user-attachments/assets/a8158992-158f-4eb2-9e79-fd7ae91008a9)

Boolean function minimization f2
![Screenshot 2024-11-20 155058](https://github.com/user-attachments/assets/2acdb7d7-8daf-4547-8a73-9dde2ab833de)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

