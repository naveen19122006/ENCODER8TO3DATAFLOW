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

Step1: Define the specifications and initialize the design.

Step2: Declare the name of the entity and architecture by using VHDL source code.

Step3: Write the source code in VERILOG.

Step4: Check the syntax and debug the errors if found, obtain the synthesis report.

Step5: Verify the output by simulating the source code.

Step6: Write all possible combinations of input using the test bench.

Step7: Obtain the place and route report.

**PROGRAM**

 Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: NAVEEN KUMAR E 

RegisterNumber:24006129

ENCODER

~~~
module encoder(d, x, y, z);
input [7:0] d;
output x;
output y;
output z;
assign x=d[4]|d[5]|d[6]|d[7];
assign y=d[2]|d[3]|d[6]|d[7];
assign z=d[1]|d[3]|d[5]|d[7];
endmodule
~~~


**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2024-11-30 223343](https://github.com/user-attachments/assets/1ee02939-c7d3-4d93-831c-08e9e7b84727)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2024-11-30 223619](https://github.com/user-attachments/assets/fd1cef4f-4036-4a23-8b33-955bb51cf22e)


**RESULTS**

Thus the OUTPUT’s of Encoder is verified by synthesizing and simulating the
VERILOG code.




