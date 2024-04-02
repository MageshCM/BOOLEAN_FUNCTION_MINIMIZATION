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
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: Magesh C M 

RegisterNumber: 212223220053
```
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```
**RTL realization**

**Output:**

![image](https://github.com/MageshCM/BOOLEAN_FUNCTION_MINIMIZATION/assets/164765537/53417b8f-9410-4fd2-aa6c-f89f40745b2c)

**Truth Table**

![image](https://github.com/MageshCM/BOOLEAN_FUNCTION_MINIMIZATION/assets/164765537/2193aec2-d646-42e0-b77f-78d44bc885bb)

**RTL**

**Timing Diagram**
![image](https://github.com/MageshCM/BOOLEAN_FUNCTION_MINIMIZATION/assets/164765537/b935c535-7d1f-4e32-aae7-53545a9ff029)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

