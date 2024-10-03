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

Developed by:yenuganti prathyusha
RegisterNumber: 212223240187
![Screenshot 2024-10-03 115838](https://github.com/user-attachments/assets/379c1655-ffba-464b-a40a-ac45d0dac0ff)
module lg(A,B,C,D,F1);
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


*/


**RTL realization**
## Truthtable
![image](https://github.com/user-attachments/assets/f4dd9ab8-d282-4ff6-b6ce-9a9a0266bb83)

**Output:**

**RTL**
![Screenshot 2024-10-03 061537](https://github.com/user-attachments/assets/e85ce2d4-962f-4fa1-ad7d-f98fc6ba9cf5)


**Timing Diagram**
![Screenshot 2024-10-03 122042](https://github.com/user-attachments/assets/839a7118-f81d-4e0b-9603-abbf0c98f194)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

