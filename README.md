# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
 
 Identity Law A ⋅ 1 = A, A + 0 = A
 
 Null Law A ⋅ 0 = 0, A + 1 = 1
 
 Idempotent Law A ⋅ A = A, A + A = A
 
 Complement Law A ⋅ A′ = 0, A + A' = 1
 
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
 
 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 
 Commutative law A B = B A,A + B = B + A

**Logic Diagram**

Identity law
![identity](https://github.com/user-attachments/assets/04af0b03-205a-4e89-8129-fd8481b13603)

Idempotent Law
![idempotent](https://github.com/user-attachments/assets/e82e17a4-41c3-4011-a676-2b850f608743)

Complement Law
![complement](https://github.com/user-attachments/assets/5d9dec2e-bb3d-4454-89a8-fd8a1aa5b8b7)

Distributive Law
![distributive](https://github.com/user-attachments/assets/8ebbe80f-ad3c-4ab5-8ea7-41fa5e0d6658)

De Morgan’s Law
![demorgans](https://github.com/user-attachments/assets/d5d469f1-3b49-4b8d-b66a-be654d08f032)

Absorption Law
![absorption](https://github.com/user-attachments/assets/6dbc38a0-bd66-4c2b-8983-bbcb9a7ccdf2)

Associative Law
![associative](https://github.com/user-attachments/assets/9aabe8b5-02f3-4828-9bfa-385b67c88add)

Commutative law
![commutative](https://github.com/user-attachments/assets/a2a3a14b-d90e-45cc-94a7-401a1c33d70d)

Null law
![null](https://github.com/user-attachments/assets/05aaab1c-272f-4eb2-90b3-7e5d60c8c9a7)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**Program:**
 Program to implement the given logic function and to verify its operations in quartus
 using Verilog programming.
 
 i)
 
 module funct1(a,b,c,d,f1);
 
 input a,b,c,d;
 
 output f1;
 
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 
 endmodule
 
 ii)
 
 module funct2(w,x,y,z,f2);
 
 input w,x,y,z;
 
 output f2;
 
 assign f2=((~y & z)|( w & y )|(x & y));
 
 endmodule


**RTL realization**

**Output:**
i)
![image](https://github.com/user-attachments/assets/2c94687d-ec0c-44b9-9391-400f03dba0c3)

2)
![image](https://github.com/user-attachments/assets/9a71c17d-2bd2-4554-99a7-b945e022558e)


**RTL**

**Timing Diagram**
i)
![image](https://github.com/user-attachments/assets/bd647b2e-3e6f-49aa-ab28-a7b042a0926b)

2)
![image](https://github.com/user-attachments/assets/18ca26c5-3ada-4805-b671-1b74fdd4021e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

