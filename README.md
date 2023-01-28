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
Developed by: NANDHINI.E
RegisterNumber: 22007762 
*/






### RTL LOGIC 
![ENCODER](https://user-images.githubusercontent.com/121998147/215265160-471abab1-e388-40c9-b580-28957534b296.png)

![DECODER](https://user-images.githubusercontent.com/121998147/215265163-af1e7812-35eb-4b1c-b374-c63bfbf48247.png)








### TIMING DIGRAMS  
![ENCODER TD](https://user-images.githubusercontent.com/121998147/215265172-3323b01b-2b91-410e-a106-a1c1b5e73c62.png)

![DECODER TD](https://user-images.githubusercontent.com/121998147/215265179-e170d5f9-f1dd-4466-b93c-8d258f7d3ff0.png)





### TRUTH TABLE 

![E TT](https://user-images.githubusercontent.com/121998147/215265401-8043585c-7e16-4d63-92ba-444eb036b24d.png)

![DEC TT](https://user-images.githubusercontent.com/121998147/215265404-5521f241-1e78-468e-9da9-7934839857e5.png)




### RESULTS 
Hence verified the encoder and decoder.....
