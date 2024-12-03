**EXP3: HALF ADDER AND SUBTRACTOR**

NAME : SARAVANA KUMAR

REF NO: 24900200

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

HALF ADDER

![image](https://github.com/user-attachments/assets/d51ec989-56fa-47af-b6a6-8d1f06a095b5)


HALF SUBRACTOR

![image](https://github.com/user-attachments/assets/7a0da64a-41ca-4bfd-a328-422069d197e8)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER

module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule


HALF SUBRACTOR

module halfsubractor(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule


**RTL Schematic**

HALF ADDER

![screen shot of half adder](https://github.com/user-attachments/assets/bbce9efd-85e6-4676-bdcd-bf783fb5077e)



HALF SUBRACTOR

![screenshot of half subractor](https://github.com/user-attachments/assets/89154c89-f4df-4109-90fb-838ef90a6827)



**Output/TIMING Waveform**

HALF ADDER


![wave form of half adder](https://github.com/user-attachments/assets/d04b76af-ece9-45f3-95ae-7a31f145873b)



HALF SUBRACTOR


![wave form of half subractor](https://github.com/user-attachments/assets/1a5ca4b9-3779-4edf-b30c-edee979df12a)


**Result:**

Thus the a half adder and half subtractor circuit is designed and  its truth table is verified in Quartus using Verilog programming.
