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
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Y.Nitheesh 
RegisterNumber:24011476


**RTL realization output**
![image](https://github.com/user-attachments/assets/a114f901-bf4e-4528-9ed1-823d5839e5eb)
![image](https://github.com/user-attachments/assets/f3b5d8a4-f160-4a87-ad58-9a4667b01e6c)

**RTL**
![image](https://github.com/user-attachments/assets/9938a2ec-ab68-4d21-88c2-fba5809f0d15)

![image](https://github.com/user-attachments/assets/edcf9240-1007-4153-855c-8f1246c5d667)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

