# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
Developed by: 
RegisterNumber:  
*/
Logic symbol & Truthtable
RTL realization

### Output:
## HALF ADDER
```
module halfhadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule
```
## FULLADDER
```
module fulladder1(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=((a^b)^c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule
```
### RTL
![so](https://user-images.githubusercontent.com/118703522/231666970-82edc516-d25c-4a84-9d4f-ff6b33c38d8e.png)
![soo](https://user-images.githubusercontent.com/118703522/231667633-93a6bf24-8cf8-4d7a-a608-00847fe70fd7.png)

### TIMING DIAGRAM
![supper](https://user-images.githubusercontent.com/118703522/231673771-241df137-86e6-4a59-989e-9e1d662b49e8.png)

![Screenshot 2023-04-13 105553](https://user-images.githubusercontent.com/118703522/231667812-d26e3e47-c746-4f4e-bcdf-134beced12af.png)

### TRUTH TABLE 
![sooo](https://user-images.githubusercontent.com/118703522/231668430-9f4f0c88-799f-477a-aec5-5884b6c22a17.png)
![output](sur.png)
### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
