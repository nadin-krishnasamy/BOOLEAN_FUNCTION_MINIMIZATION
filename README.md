# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
'''  

module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule

'''

Developed by: NADIN KRISHNASAMY B / RegisterNumber: 25016795 

**RTL realization Output**

<img width="1175" height="607" alt="Screenshot 2025-12-10 214220" src="https://github.com/user-attachments/assets/70cf84fc-56b9-4fc2-8d73-25cbf7c614a7" />

**RTL**

<img width="1175" height="594" alt="Screenshot 2025-12-10 214244" src="https://github.com/user-attachments/assets/c062ed52-52c8-49ee-827d-59634b57f3c0" />

**Timing Diagram**

![EXP 2](https://github.com/user-attachments/assets/a1e74d77-9a33-4dbc-8889-a22501a20b93)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

