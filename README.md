# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.
Developed by:N.Swetha
RegisterNumber:22008828 
*/






### RTL LOGIC  

![encoder RTL](https://user-images.githubusercontent.com/122199934/214796019-a38bfa3d-e547-4c39-a5a1-08bd89508c7e.png)

![decoder RTL](https://user-images.githubusercontent.com/122199934/214796098-1605380e-33bd-4304-bbf8-a8bdd099f092.png)







### TIMING DIGRAMS  


![encoder simulation](https://user-images.githubusercontent.com/122199934/214796203-ca359405-6038-4e80-931c-4b1ee402358a.png)

![decoder simulation](https://user-images.githubusercontent.com/122199934/214796152-866c9193-e770-4294-aca1-3e8f40eeaaac.png)




### TRUTH TABLE 

ENCODER:

![image](https://user-images.githubusercontent.com/122199934/214796330-887e9d4a-bf2b-4a6b-a4f0-ab55d97c5604.png)


DECODER:

![image](https://user-images.githubusercontent.com/122199934/214796489-c2b253f2-d920-4021-b078-c8454ecf6587.png)






### RESULTS 

Thus the Encoder and Decoder circuits are designed and truth table are verified using quarts
