## Date :
## Ex No:02- Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```python
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: SANJAY M
RegisterNumber:23013084

module ex_02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```


## RTL realization:
![Screenshot 2023-12-20 083419](https://github.com/sanjayofficial2005/Experiment--02-Implementation-of-combinational-logic-/assets/148048602/1f27fb34-9ac6-4f2d-8eae-2e1bda5a30e9)


## Truth table:
![Screenshot 2023-12-20 083406](https://github.com/sanjayofficial2005/Experiment--02-Implementation-of-combinational-logic-/assets/148048602/1a45f12d-cb06-4193-ac1c-2a1d764fc29e)


## Timing Diagram:
![Screenshot 2023-12-20 083431](https://github.com/sanjayofficial2005/Experiment--02-Implementation-of-combinational-logic-/assets/148048602/a51d8eb3-5817-4b8e-bfe6-45fcc5d670fc)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
