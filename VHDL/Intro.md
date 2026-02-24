VHDL Introduction

#### Table of Contents  
[Headers](#headers)  
[Emphasis](#emphasis)  
...snip...    
<a name="headers"/>
## Headers
### Design of a Circuit Represented As a Boolean Function Using VHDL Code

```
Example1: Complete VHDL design for the function F1 = (A'.B.C') + (B'.C) + (A'.B)
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
