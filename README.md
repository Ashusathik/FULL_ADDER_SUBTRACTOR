# EXPT 4 FULL_ADDER_SUBTRACTOR
DATE:19/10/2024
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

**Truthtable full adder
![Screenshot 2024-12-26 220028](https://github.com/user-attachments/assets/4376f596-9b9e-4cd4-9828-6a341aaa62fc)

full subtractor
![Screenshot 2024-12-26 220204](https://github.com/user-attachments/assets/e8b23aef-1c54-4438-a7f8-96bd0c2fe8a2)

**Procedure**

Full adder A full adder is a combinational logic circuit that adds three one-bit binary numbers to produce a two-bit output. The output is the sum and the carry value. The truth table for a full adder can be used to implement the full adder logic. Full subtractor A full subtractor is a combinational circuit that performs subtraction involving three bits: A (minuend), B (subtrahend), and Bin (borrow-in). It produces two outputs: D (difference) and Bout (borrow out).

**PrograFull Adder module adder(a,b,cin,sum,carry); input a,b,cin; output sum,carry; assign sum=( (a ^ b)^cin); assign carry= ( (a & b)| ( cin &(a ^ b ))); endmodule

Full Subtractor module subtractor(a,b,bin,difference,borrow); input a,b,bin; output difference,borrow; assign difference= ( (a ^ b)^bin); assign borrow= ( ( a & b)| ( bin & ((a ^ b )))); endmodulem:


/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:ASHRATHI S RegisterNumber:24900260
*/

**RTL Schematic
FULL ADDER
![Screenshot 2024-12-26 220256](https://github.com/user-attachments/assets/0b6025a0-5c12-4834-a1b7-463587a1f517)
FULL SUBTRACTOR
![Screenshot 2024-12-26 220410](https://github.com/user-attachments/assets/1be356bf-0fa3-4a5d-9ab8-e54b41af9805)
FULL SUBTRACTOR
![Screenshot 2024-12-26 220451](https://github.com/user-attachments/assets/4ccf8e50-e0d8-4040-b835-76acaba50fba)


**Output Timing Waveform
Full Adder
![Screenshot 2024-12-26 220535](https://github.com/user-attachments/assets/abfcf66b-322f-4731-8059-ca7d4c1e45d5)
Full Subtrator
![Screenshot 2024-12-26 220622](https://github.com/user-attachments/assets/bf28fb09-4c9f-4cda-98c4-2e8ba3670641)


**Result:Thus the Full Adder and Full Subttractor circuits are designed and the truth is verified using Quartus software

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



