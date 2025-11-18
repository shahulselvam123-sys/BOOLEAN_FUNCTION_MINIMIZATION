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
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;

assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));
assign f2 = ((~y & z) | (w & y) | (x & y));

endmodule
```

**RTL realization**



<img width="1920" height="1080" alt="Screenshot 2025-11-18 112232" src="https://github.com/user-attachments/assets/3e079d1d-8ca9-4706-8260-c1d66f715682" />

**Output:**
*<img width="1920" height="1080" alt="Screenshot 2025-11-18 113253" src="https://github.com/user-attachments/assets/a0cb587b-90dc-4e1a-859f-49b9154dcc05" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

