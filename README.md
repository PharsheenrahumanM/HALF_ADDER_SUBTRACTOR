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



Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B



Figure -02 HALF Subtractor


**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.


Developed by: RAMASRI K

RegisterNumber:24007403

module Halfadd(a,b,sum,carry);

input a,b;


output sum,carry;

assign sum=(a^b);

assign carry=(a&b);

endmodule

module Halfsub(a,b,diifference,borrow);

input a,b;

output difference,borrow;

assign difference=(a^b);

assign borrow=(~a&b);

endmodule


**RTL Schematic**

![Screenshot 2025-04-23 154225](https://github.com/user-attachments/assets/e287bb9a-3477-40b3-86c5-a743a82f2af5)

![DE3SUBD](https://github.com/user-attachments/assets/ebe7e424-fba6-4499-889b-ccf562af7cdf)



**Output/TIMING Waveform**
![Screenshot 2025-04-23 153100](https://github.com/user-attachments/assets/88387ea5-ca22-40e3-93b8-feb84367a80d)


![DE3OUTSUB](https://github.com/user-attachments/assets/e3858436-d99c-4fb2-b7f1-ddf50f4f2517)





**Result:** Thus the given program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
