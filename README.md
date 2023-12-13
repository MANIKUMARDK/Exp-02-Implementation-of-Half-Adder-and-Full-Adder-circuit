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

### Procedure:Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.


### 
Program:Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:MANIKUMAR D.K
RegisterNumber:23013588

1.1.Program to design a half adder:
module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule

1.1.Program to design a full adder:
module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
Logic symbol & Truthtable
### RTL realization : HALF ADDER: ![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/f243d309-98f0-4c6b-ad8f-46e544ed845c)
### RTL realisation : FULL ADDER: ![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/5821cbef-0e8d-42da-9ccd-b44d417a4931)


### Output:
### RTL
### TIMING DIAGRAM: HALF ADDER :![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/0e9d1c9c-c608-4a05-b639-115cb9e80056)
### TIMING DIAGRAM: FULL ADDER ![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/9a395b96-8418-448c-b59e-282ca5d1bf68)



### TRUTH TABLE HALF ADDER :![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/eb4e49b0-0a33-4d23-be6b-9d2b2ccde132)
### TRUTH TABLE FULL ADDER:![image](https://github.com/MANIKUMARDK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147215581/f9aea43f-9cd1-4af6-8d0c-9670a3fa8954)


### Result:
