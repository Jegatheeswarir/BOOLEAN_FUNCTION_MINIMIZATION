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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: JEGATHEESWARI R

RegisterNumber: 212223230092

```
module program2(A,B,C,D,F1);
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

![exp2rtl](https://github.com/Jegatheeswarir/BOOLEAN_FUNCTION_MINIMIZATION/assets/144871077/cc27fd29-f308-4008-819c-88e97edd7a68)

**Truth table**

![truth2](https://github.com/Jegatheeswarir/BOOLEAN_FUNCTION_MINIMIZATION/assets/144871077/d2724ae7-2e63-4420-ac42-f8fd8ef3edde)


**Timing Diagram**

![waveform2](https://github.com/Jegatheeswarir/BOOLEAN_FUNCTION_MINIMIZATION/assets/144871077/bae5ba1b-aad9-4262-8147-05bd2884bcb6)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

