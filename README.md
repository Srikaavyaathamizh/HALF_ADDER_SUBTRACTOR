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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: SRIKAAVYAA T

RegisterNumber: 212223230214*/


## Half_adder program:
```
module halfadd_top(a,b,sum,carry);
input a,b; 
output sum,carry; 
assign sum = a^b; 
assign carry = a & b; 
endmodule

```

## Half_subtractor program:
```
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo;
// Outputs sum and carry for half adder:Outputs difference D,Borrow Bo for half subtractor
assign D = a ^ b;
assign Bo = ~a & b;
endmodule
```

![Screenshot 2024-10-17 223834](https://github.com/user-attachments/assets/5b6dd1a6-e610-419e-80e2-d273ddff7f69)

![Screenshot 2024-10-17 223842](https://github.com/user-attachments/assets/14797337-fbe2-4f1c-b6d3-e8c7179b0af8)

## Half_adder

![Screenshot 2024-10-17 224016](https://github.com/user-attachments/assets/9bfff17f-20c1-4ac0-9a5c-f33a2697e671)


## Half_subtractor

![Screenshot 2024-10-17 224022](https://github.com/user-attachments/assets/8f02557b-d543-4846-b54c-d3ed9e0ab9fd)


**Output/TIMING Waveform**

## Half_adder

![Screenshot 2024-10-17 224245](https://github.com/user-attachments/assets/5d573b4c-5ffb-4133-84c3-b17a6b6c3390)

## Half_subtractor

![Screenshot 2024-10-17 224259](https://github.com/user-attachments/assets/7a42a3ce-26a9-447b-92da-3c03f51c9161)

**Result:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming its are verifid
