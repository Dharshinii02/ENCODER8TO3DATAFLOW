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

An encoder is a digital circuit that converts a set of binary inputs into a unique binary code. The binary code represents the position of the input and is used to identify the specific input that is active. Encoders are commonly used in digital systems to convert a parallel set of inputs into a serial code. The basic principle of an encoder is to assign a unique binary code to each possible input. For example, a 2- to-4 line encoder has 2 input lines and 4 output lines and assigns a unique 4-bit binary code to each of the 2 ^ 2 = 4 possible input combinations. The output of an encoder is usually active low, meaning that only one output is active (low) at any given time, and the remaining outputs are inactive (high). The active low output is selected based on the binary code assigned to the active input. There are different types of encoders, including priority encoders, which assign a priority to each input, and binary- weighted encoders, which use a binary weighting system to assign binary codes to inputs. In summary, an encoder is a digital circuit that converts a set of binary inputs into a unique binary code that represents the position of the input. Encoders are widely used in digital systems to convert parallel inputs into serial codes. An Encoder is a combinational circuit that performs the reverse operation of a Decoder. It has a maximum of 2 ^ n input lines and 'n' output lines, hence it encodes the information from 2^n inputs into an n-bit code. It will produce a binary code equivalent to the input, which is active High. Therefore, the encoder encodes 2^n input lines with 'n' bits

**PROGRAM**

```
module EX5(din,a,b,c);
input[0:7]din;
output a;
output b;
output c;
assign a= din[4]|din[5]|din[6]|din[7];
assign b= din[2]|din[3]|din[6]|din[7];
assign c= din[2]|din[4]|din[6]|din[7]; 
endmodule
```



**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2025-05-07 151716](https://github.com/user-attachments/assets/9884d069-2223-41e7-a00c-34a799681d77)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2025-05-07 151734](https://github.com/user-attachments/assets/3f03dc13-5f0e-4db6-a609-c849d1f2adf4)
# Developed by: Dharshini J
# RegisterNumber:212224240036


**RESULTS**



Therefore encoder 8 to 3 in dataflowing modeling using verilog and validating their functionally using their functional tables is verify.
