<img width="806" height="409" alt="image" src="https://github.com/user-attachments/assets/1cb18ec0-c874-4c25-b348-a1cff25869f3" /><img width="806" height="409" alt="image" src="https://github.com/user-attachments/assets/1cb18ec0-c874-4c25-b348-a1cff25869f3" />VHDL Introduction

#### Table of Contents  
[Headers](#headers)  
[Emphasis](#emphasis)  
...snip...    
<a name="headers"/>
## Headers
### Design of a Circuit Represented As a Boolean Function Using VHDL Code

```
Example1: Complete VHDL design for the function F1 = (A'.B.C') + (B'.C) + (A'.B)
```
```
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;
entity comb1 is port (
A, B, C : in std_logic;
F1 : out std_logic
);
end comb1;
architecture Boolean_function of comb1 is
begin
F1 ,5 (not A and B and not C) or (not B and C) or (A and not B);
end Boolean_function;
```

```
Shows a complete VHDL design for the 2-to-4 decoder
```
```
Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://drive.google.com/file/d/1iDV4nt33293GPB9vM2l36aomciO1bLVR/view?usp=drive_link "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://drive.google.com/file/d/1gRVcC8uKoDCX1_M1RI23xlZHtzq9_A7_/view?usp=drive_link "Logo Title Text 2"
```
```
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;
entity comb6 is port (
B1, B0 : in std_logic;
F0, F1, F2, F3 : out std_logic
);
end comb6;
architecture Boolean_functions of comb6 is
begin
F0 ,5 not B1 and not B0;
F1 ,5 not B1 and B0;
F2 ,5 B1 and not B0;
F3 ,5 B1 and B0;
end Boolean_functions;
```
