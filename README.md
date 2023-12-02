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

1.create module encoder and decoder.

2.Get inputs and outputs for encoders and decoders.

3.perform or operation for encoder and and logic for decoders.

4.perform RTL LOGIC and get waveform.

### PROGRAM 
Encoder:

![Screenshot 2023-12-02 162503](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/3efdec8f-c47d-41c9-8998-1e8930430d53)

Decoder:

![Screenshot 2023-12-02 162655](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/7c8864d3-b977-4287-8ad8-f154fae9fc10)

### RTL LOGIC  
Encoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/0ef6331d-7f34-459d-ad4d-3cef6a9a5b8d)

Decoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/d07e7a9e-3616-4adf-b75c-1446406e015e)

### TIMING DIGRAMS  
Encoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/2d23cb7a-9fdb-4909-83c9-9e43a2ecda2e)

Decoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/795c38cc-c705-4f60-8179-48d8b285dbdb)

### TRUTH TABLE 
Encoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/7c2e11a9-9254-4dc8-aafb-990af472da26)

Decoder:

![image](https://github.com/Devadhaarini/Experiment-08-Encoders-and-decoders-/assets/145796552/f01ed5c6-6de3-4b4e-8349-aa024ac6348c)

### RESULTS 
Thus the program to design encoder and decoder is done.
