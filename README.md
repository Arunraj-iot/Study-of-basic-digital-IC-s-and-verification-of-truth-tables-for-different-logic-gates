### Study-of-Basic-Gates

## Name: arunraj R
## Reg no: 212224110006
**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as,

    - AND gate 
    - OR gate 
    - NOT gate 

                * NAND gate 
                * NOR gate 

                            1. Ex-OR gate 
                            2. Ex-NOR gate

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

Program for logic gates and verify its truth table in quartus using Verilog programming
```verilog
module logic_gates(
    input a, b,
    output not_a,
    output and_ab,
    output or_ab,
    output nand_ab,
    output nor_ab,
    output xor_ab,
    output xnor_ab
);

assign not_a   = ~a;          // NOT gate for 'a'
assign and_ab  = a & b;       // AND gate
assign or_ab   = a | b;       // OR gate
assign nand_ab = ~(a & b);    // NAND gate
assign nor_ab  = ~(a | b);    // NOR gate
assign xor_ab  = a ^ b;       // XOR gate
assign xnor_ab = ~(a ^ b);    // XNOR gate

endmodule

```

```
Developed by    : Arunraj r
Register Number : 212224110006
```

**Logic symbol & Truthtable**

![image](https://github.com/user-attachments/assets/32761285-db9c-47bd-9900-f2cf3e794c90)

![image](https://github.com/user-attachments/assets/b41d893c-5ab0-4d3d-a00a-9155dabd2c00)


**RTL realization Output:** 

![image](https://github.com/user-attachments/assets/e31629fb-a480-4c52-a370-24df7c08f69f)

**OUTPUT:**
Timing Waveform

![image](https://github.com/user-attachments/assets/9dcaed88-13c7-49f9-b5ed-cf62a9db0a11)



**Result:**

The truth table of logic gates in Quartus II using Verilog programming is verified.
