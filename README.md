# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
1)FULL ADDER
![image](https://github.com/user-attachments/assets/2b35bb13-24d0-45e6-91b3-85ce80917fd6)

2)FULL SUBTRACTOR
![image](https://github.com/user-attachments/assets/fd69421d-a791-43d9-864c-62bd0a22ac47)



**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming
1)FULL ADDER
module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule

2)FULL SUBTRACTOR
module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule


. Developed by: RegisterNumber:
*/

**RTL Schematic**
1)FULL ADDER
![Screenshot 2024-12-01 153117](https://github.com/user-attachments/assets/f3104eb0-6000-4d80-b2ae-c8b111dde8cd)

2)FULL SUBTRACTOR
![Screenshot 2024-12-03 194701](https://github.com/user-attachments/assets/23cb9b7e-f887-4573-a4c9-4dc9c8ae4062)




**Output Timing Waveform**
1)FULL ADDER
![Screenshot 2024-12-01 153445](https://github.com/user-attachments/assets/a2fe1dad-22e9-4cb1-8e0b-ab14bb90ab85)

2)FULL SUBTRACTOR
![Screenshot 2024-12-03 195003](https://github.com/user-attachments/assets/a734cb40-aff1-426e-b41d-975870156eb9)




**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



