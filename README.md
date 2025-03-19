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


```
module ex2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,x,y,z,w;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&(~c)&(~d))|((~b)&c&d)|((~a)&b&c&d)|(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|((~w)&x&y)|(w&(~x)&y)|(w&x&y);
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber: Ramya G(212224220078)


DATE: 18/03/2025


**RTL realization**

**Output:**

![Screenshot 2025-03-19 015334](https://github.com/user-attachments/assets/e4cc0cbd-dda6-455c-b40f-d95766ec4a5a)


**RTL**


![Screenshot 2025-03-19 014551](https://github.com/user-attachments/assets/5d9955ca-20bf-4393-aa43-83d67198713f)



**Timing Diagram**


![Screenshot 2025-03-19 014506](https://github.com/user-attachments/assets/ea09b828-c0b6-4727-90f7-04b97d39a401)


**Result:**

Thus the given truth table of logic gate are successfully in QUATRUS II by using verilog HDL programming

