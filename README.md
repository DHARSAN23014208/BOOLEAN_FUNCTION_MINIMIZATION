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
~~~
module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
~~~

Developed by:DHARSANKUMAR R RegisterNumber:212223240028


**RTL realization**

![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/e8495c09-7b03-492b-b9ef-5a70e398394f)


**TRUTH TABLE**

![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/4e3baf11-5d56-4c6f-9e4a-0f019618966a)



**Timing Diagram**

![image](https://github.com/DHARSAN23014208/BOOLEAN_FUNCTION_MINIMIZATION/assets/149365413/99b38dc2-7fd6-41d7-bc1d-830d13f8c753)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

