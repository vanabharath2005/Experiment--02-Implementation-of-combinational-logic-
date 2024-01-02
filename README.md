
# Experiment 02: Implementation of combinational logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
### Hardware – PCs, Cyclone II , USB flasher
### Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
````
module kmap(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire A1,A2,A3,B1,B2,B3;
assign A1=(~a&(~b)&(~c)&(~d));
assign A2=(a&c&(~d));
assign A3=((~b)&c&(~d));
assign F1=A1|A2|A3;
assign B1=(x&(~y)&z);
assign B2=(~x&(~y)&z);
assign B3=(~w&x&y);
assign F2=B1|B2|B3;
endmodule
````
## RTL realization

![image](https://github.com/vanabharath2005/Experiment--02-Implementation-of-combinational-logic-/assets/147222071/94dbc144-b4ee-478d-bb9d-5a4fca3ee56b)
TRUTH TABLE

![image](https://github.com/vanabharath2005/Experiment--02-Implementation-of-combinational-logic-/assets/147222071/477e13d6-9b2d-4edb-af74-db7e1716b558)

WAVE FORM

![image](https://github.com/vanabharath2005/Experiment--02-Implementation-of-combinational-logic-/assets/147222071/b0e1101c-6722-4174-8555-860178fe1bff)

## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
