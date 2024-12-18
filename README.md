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

![WhatsApp Image 2024-12-18 at 10 28 49_50506500](https://github.com/user-attachments/assets/9e32b05a-dc56-4b94-9a59-2f708da8b6af)
 
      


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
~~~
module experiment2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~c) | (~a&b&d) | (a&b&~c));
assign f2=((~y&z) | (x&y) | (w&y));
endmodule
~~~
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: priyesh s
RegisterNumber:* 24008184


**RTL realization** 

![395801703-40779e5e-0ee0-4ac7-a567-efa9a91ba74d](https://github.com/user-attachments/assets/fa93b06d-9860-4371-bc9a-faac2a9e7fdd)
![395801740-e8d53050-3042-4a72-9cdf-ecf84545daef](https://github.com/user-attachments/assets/e1fb1933-5d60-4424-8331-fd1659c68686)

**Timing Diagram** 

![395801643-339929cb-6907-49a5-baf1-f5dbc897def4](https://github.com/user-attachments/assets/cb2f3a4a-b3f7-4bc8-a93c-c1c4f337166b)
![395801667-85cdd59f-7b41-4e0b-b272-deb9fbc30a54](https://github.com/user-attachments/assets/621bf9b4-0763-410b-9fc0-fe745da66ae7)



**Result:** The Basic logic gates are studied and truth table are verified.

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

