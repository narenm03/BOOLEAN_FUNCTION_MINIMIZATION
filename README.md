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
//Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:NARENDHARAN.M RegisterNumber:212223230134

module booleanfunction(a,b,c,d,w,x,y,z,f1,f2);
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
and G1(s,ydash,z);
and G2(t,x,y);
and G3(u,w,y);
or G4(f2,s,t,u);
endmodule

```

![image](https://github.com/narenm03/BOOLEAN_FUNCTION_MINIMIZATION/assets/152469427/a1b896fc-aa8e-4df2-94a2-353ac7969625)

**RTL realization**

![Screenshot 2024-03-18 102835](https://github.com/Hashwatha/BOOLEAN_FUNCTION_MINIMIZATION/assets/150231431/d59fa67a-d1dc-4543-8ffc-54d8a1ee34f9)

**Output:**

![Screenshot 2024-03-18 103758](https://github.com/Hashwatha/BOOLEAN_FUNCTION_MINIMIZATION/assets/150231431/97fff674-8fef-446c-9d38-449d3fb437a9)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

