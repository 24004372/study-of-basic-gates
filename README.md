### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**
```
Program for logic gates and verify its truth table in quartus using Verilog programming

 Developed by: SHRIRAM VR
 
 RegisterNumber: 24004372
```

```
module logicgate(a,b,c);
 input a;
 input b;
 output [6:0] c;
 
 
       assign c[0]=a&b;
		 assign c[1]=a|b;
		 assign c[2]=~(a&b);
		 assign c[3]=~(a|b);
		 assign c[4]=a^b;
		 assign c[5]=~(a^b);
		 assign c[6]=~a;
		 
endmodule

```
 
**Logic symbol & Truthtable**
![428277522-d813e0f3-5f62-4249-9bdf-fdaa16f94298](https://github.com/user-attachments/assets/ef902800-2af9-40ce-a1b4-4a15093f1ff3)




**RTL**

![428277542-385f0df0-3ae2-4afa-933c-7f92814ada01](https://github.com/user-attachments/assets/a4ee8d5a-2731-4536-befa-d225e62b8746)



**Result:**
Thus the basic logic gates are studied and the ttruth tables are verified


