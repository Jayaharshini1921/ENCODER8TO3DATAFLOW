### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**

module encodder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0 = d1|d3|d5|d7;
assign a1 =d2|d3|d6|d7;
assign a2 =d4|d5|d6|d7;
endmodule

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:jayaharshini s RegisterNumber:212224100024
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2025-04-29 155846](https://github.com/user-attachments/assets/fd6b2ab4-12d4-4726-8f29-caab64683849)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2025-04-29 155852](https://github.com/user-attachments/assets/3b607acc-f03e-49c4-ac1c-83de2ea077a6)

**RESULTS**
Thus the code is executed successfully.



