# NAME: DEEPAK
# REFERENCE NO: 23000154
# Exp 03 Implementation of Half Adder and Full Adder circuit
# Implementation of HalfAdder and FullAdder circuit
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

#### Figure  01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure  02 FULL ADDER 

### Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
# Program:

Half adder:
module exp3(sum, carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
full adder:
module fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
# RTL realization:
# HALF ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/3ae06048-794b-496c-b0ad-b08b54f7592c)
# FULL ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/5feb2796-68a4-45a9-b536-a45a50859602)





### TIMING DIAGRAM:
# HALF ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/5a14c0a2-2d73-48c4-959d-ba88284128f9)

# FULL ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/a048e2c3-d21e-4b9e-8f3d-79c36992522a)


### TRUTH TABLE:
# HALF ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/afec5015-2acd-499c-b315-05559f9bcca1)


# FULL ADDER:
![image](https://github.com/deepak23000154/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151951350/13c4aa72-936d-4602-b7a6-b717ec059337)


### Result:
