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
Developed by: BHUVANESH.S.R
RegisterNumber:212223240017
//Verilog model: Circuit with Boolean expressions
module ex2(F1,F2,A,B,C,D);
output F1,F2;
input A,B,C,D;
assign F1=(~A&~B&~C&~D)|(A&~C&~D)|(~B&C&~D)|(~A&B&C&D)|(B&~C&D);
assign F2=(B&~C&D)|(~B&~C&D)|(~A&B&C)|(A&~B&C)|(A&B&C);
endmodule
```

**Output:**

![Screenshot 2024-03-12 151457](https://github.com/Bhuvanesh-Suresh/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742661/1a42e460-893f-4ef0-aca7-b110a8cf9b88)
![output new](https://github.com/Bhuvanesh-Suresh/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742661/de72918f-c266-4030-b63c-2bc7ff263fb2)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

