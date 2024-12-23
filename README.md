**DATE:**8|10|24.

# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

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

![Screenshot 2024-12-23 142009](https://github.com/user-attachments/assets/a3c843c9-875a-4771-a7aa-c7ab4609bf42)


![Screenshot 2024-12-23 142030](https://github.com/user-attachments/assets/d808fc94-eaab-4b55-88a4-36efaf092ed8)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

~~~

i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
~~~
~~~
ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
~~~

Developed by:GURUPARAN G RegisterNumber:*24001677

**RTL Schematic**

![Screenshot 2024-12-23 140316](https://github.com/user-attachments/assets/4274008f-e1bd-4c13-9760-e63a85180e53)


![Screenshot 2024-12-23 141243](https://github.com/user-attachments/assets/7489d924-47ec-4e09-a3a7-60be6de35786)

**TIMINING WAVEDIAGRAM**

![Screenshot 2024-12-23 140542](https://github.com/user-attachments/assets/d727661d-a207-4986-a294-8676aa61e612)

![Screenshot 2024-12-23 141427](https://github.com/user-attachments/assets/8e3899c2-e0a9-4c31-bbf5-a3412190d7c5)

**Result:**


The design of a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.
