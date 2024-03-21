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

module boolean(A,B,C,D,F1); 
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

![Screenshot 2024-03-18 102801](https://github.com/Hashwatha/BOOLEAN_FUNCTION_MINIMIZATION/assets/150231431/652a2a6a-2275-4ce4-8205-426fb9d556e8)

**RTL realization**

![Screenshot 2024-03-18 102835](https://github.com/Hashwatha/BOOLEAN_FUNCTION_MINIMIZATION/assets/150231431/d59fa67a-d1dc-4543-8ffc-54d8a1ee34f9)

**Output:**

![Screenshot 2024-03-18 103758](https://github.com/Hashwatha/BOOLEAN_FUNCTION_MINIMIZATION/assets/150231431/97fff674-8fef-446c-9d38-449d3fb437a9)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

