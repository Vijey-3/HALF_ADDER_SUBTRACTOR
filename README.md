# HALF_ADDER_SUBTRACTOR
Implementation-of-Half-Adder-and-Half Subtractor-circuit

```
Developed by: VIJEY K S
RegisterNumber:212223040239
```


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

**HALF ADDER**

![image](https://github.com/user-attachments/assets/241a5888-c899-4a31-af02-a4aee8e44484)

**HALF SUBTRACTOR**

![image](https://github.com/user-attachments/assets/edb13281-d8bc-47b6-bf14-b9e6a5b32247)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
Half Adder
module Exp_3HA (a,b,Sum,Carry);

input a,b;
output Sum, Carry;

assign Sum= (a^b);
assign Carry= (a&b);

endmodule
```
```
Half Subtractor
module Exp_3HS (a,b, diff,borr);

input a,b;
output diff, borr;

assign diff= (a^b);
assign borr= (~a&b);

endmodule
	
```

**RTL Schematic**
![image](https://github.com/user-attachments/assets/7356f67f-d81d-4315-913e-4b85845dae6b)

![image](https://github.com/user-attachments/assets/cf0ceead-046e-4d4b-9646-11274f61c0a0)


**Output/TIMING Waveform**

![image](https://github.com/user-attachments/assets/34c46381-4857-4e10-9d81-559f2defc73f)

![image](https://github.com/user-attachments/assets/b1378edf-b325-4138-9bd0-6d3604090b41)

**Result:**

Thus, the program was successfully verified.
