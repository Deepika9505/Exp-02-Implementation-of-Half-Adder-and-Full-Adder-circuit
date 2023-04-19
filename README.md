# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER

module HalfAdder(a,b,sum,carry);
input ab;
output sum,carry;
xor(sum,ab);
and(carry,a,b);
endmodule

FULL ADDER

moule FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)|^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

Developed by: K.DEEPIKA
RegisterNumber: 212222050009
*/


Logic symbol
![LS](https://user-images.githubusercontent.com/128984662/233136896-4326e26a-56e8-4b43-803b-cd3658c77de0.jpeg)



RTL realization
Output:

HALF ADDER

![HA](https://user-images.githubusercontent.com/128984662/233137873-bfac9988-4643-4fed-bb57-781c3749f3f8.jpeg)

FULL ADDER

![FA](https://user-images.githubusercontent.com/128984662/233138040-d5b369be-5ec4-4078-935f-28c00559efb9.jpeg)

RTL
TIMING DIAGRAM

HALF ADDER

![hat](https://user-images.githubusercontent.com/128984662/233138275-f3a0b861-9ce2-4a41-8448-e2c74906a7a9.jpeg)

FULL ADDER

![fat](https://user-images.githubusercontent.com/128984662/233138378-ed16fb9f-b855-41c0-9fc2-f23e6e874bdf.jpeg)

TRUTH TABLE

HALF ADDER


![hatt](https://user-images.githubusercontent.com/128984662/233138486-26fdcbf5-a3ca-40f6-976d-94926add5cf9.jpeg)

FULL ADDER

![fatt](https://user-images.githubusercontent.com/128984662/233138557-374cb767-0c51-4a0b-8fcf-96647efbf57b.jpeg)



### Result: Thus the implementation of Halfadder Fulladder Circuit are studied and the truthtable for differrent logic gates are verified
