

# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

DATE:8|10|24.

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**


![Screenshot 2024-12-27 094901](https://github.com/user-attachments/assets/a11a48a6-13e1-4a75-9f88-e40810b60828)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

~~~

Developed by:GURUPARAN G
RegisterNumber:*24001677
~~~

**Program:**

~~~

*Half_adder*
module halfadd_top(a,b,sum,carry);
input a,b;
output sum,carry; 
 assign sum = a^b;
 assign carry = a & b;
endmodule

*Half_subtractor*
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo; // Outputs sum and carry for half adder:Outputs difference D,Borrow Bo for half subtractor
assign D = a ^ b;
  assign Bo = ~a & b;
endmodule



~~~






**RTL Schematic**

HALF ADDER:
![Screenshot 2024-12-27 101043](https://github.com/user-attachments/assets/771cd95b-ef8e-4ecd-977d-08ed82613df9)

HALF SUBRACTED:
![Screenshot 2024-12-27 101058](https://github.com/user-attachments/assets/6c4560df-e315-4ba0-804c-79e6d9ed166e)



**TIMING  WAVEDIAGRAM**
HALF ADDER:
![Screenshot 2024-12-27 101115](https://github.com/user-attachments/assets/5273c752-6b27-48ba-ab29-3ef32424e5d4)

HALF SUBRACTED:
![Screenshot 2024-12-27 101130](https://github.com/user-attachments/assets/a558692f-956e-4de7-b681-881bd8a51220)



**Result:**


The design of a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.
