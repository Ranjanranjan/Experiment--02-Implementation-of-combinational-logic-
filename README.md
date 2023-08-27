 Name: Ranjan K

 Reg.No:212222230116

# Experiment-02 Implementation of combinational logic
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Using AND gate:
An AND gate is a fundamental digital logic gate that performs a logical conjunction on its input signals. It produces an output signal only when all of its input signals are high (logic level 1). If any of the input signals is low (logic level 0), the output of the AND gate remains low.

using NOT gate:
A NOT gate, also known as an inverter, is a basic digital logic gate that performs the operation of negation on its input signal. In other words, it produces the opposite (complementary) output to its input. If the input is high (logic level 1), the output will be low (logic level 0), and if the input is low, the output will be high.

using OR gate:
An OR gate is a fundamental digital logic gate that performs a logical disjunction on its input signals. It produces an output signal when at least one of its input signals is high (logic level 1). The output remains low only if all input signals are low (logic level 0).

## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:
```
Name         : Ranjan K
Register No. :212222230116
module EX02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1 = (~A) & (~B) & (~C) & (~D);
assign x2 = (A) & (~C) & (~D);
assign x3 = (~B) & (C) & (~D);
assign x4 = (~A) & (B) & (C) & (D);
assign x5 = (B) & (~C) & (D);
assign F1 = x1 | x2 | x3 | x4 | x5;
```
## RTL:
![WhatsApp Image 2023-08-26 at 09 57 36](https://github.com/Ranjanranjan/Experiment--02-Implementation-of-combinational-logic-/assets/130027697/92781469-d662-4b68-931a-f37fc5040c35)


## Truth table
![image](https://github.com/Thenmozhi-Palanisamy/Experiment--02-Implementation-of-combinational-logic-/assets/95198708/b280551a-f504-449b-8050-3c61de9a5b15)

## output waveform

![WhatsApp Image 2023-08-26 at 09 53 01](https://github.com/Ranjanranjan/Experiment--02-Implementation-of-combinational-logic-/assets/130027697/31ce2c03-a9a2-466b-a56f-f3869ff84f2d)



## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
