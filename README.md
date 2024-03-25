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
## program
## module combinationalcircuit(A,B,C,D,F1);
## input A,B,C,D;
## output F1;
## wire x1,x2,x3,x4,x5;
## assign x1=(~A)&(~B)&(~C)&(~D);
## assign x2=(A)&(~C)&(~D);
## assign x3=(~B)&(C)&(~D);
## assign x4=(~A)&(B)&(C)&(D);
## assign x5=(B)&(~C)&(D);
## assign F1=x1|x2|x3|x4|x5;
## endmodule 


Developed by:DHARSANKUMAR R RegisterNumber:212223240028


**RTL realization**
![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/dfd3b507-e1e4-4041-ba3e-da2889b008be)

**TRUTH TABLE**
![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/47fd0f8a-aad0-4d4c-85cf-31ebb61b11cc)


**Timing Diagram**
![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/64209992-5fb8-4fa1-8de5-5ce8af62c5d7)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

