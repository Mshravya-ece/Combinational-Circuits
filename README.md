# Combinational-Circuits

In this repository, I shall share some combinational circuit schematics which I have implemented in Cadence Virtuoso.

2X1 MUX

A 2x1 mux takes 2 inputs and, based on the selection line, either one of the inputs is transmitted as output. The 2x1 mux can be designed using 2 transmission gates. When the selection line ‘sel’ is active low, then nmos and pmos of upper transmission gate get ON and the input I0 is transmitted as output but when ‘sel’ is active high, the nmos & pmos transistors of lower transmission gate get ON and input I1 becomes the output.

<img width="652" height="394" alt="image" src="https://github.com/user-attachments/assets/6ca8fd09-3963-4af8-bd64-74db2dc8e5b4" />

Symbol of 2x1 mux is created as shown below in testbench circuit.

<img width="494" height="345" alt="image" src="https://github.com/user-attachments/assets/83037964-8a85-4e01-bdc8-61659bfcfe06" />

On simulation, the output is obtained.

<img width="940" height="335" alt="image" src="https://github.com/user-attachments/assets/8a51286d-e4e2-47a0-94c6-6966f770b16f" />

The average power consumed by a 2x1 mux is 2.59 μW, and the delay is 11.9 picoseconds.

4X1 MUX

4x1 mux takes 4 inputs (I0, I1, I2, I3) and based on the selection lines (S0,S1), the output is obtained. Using lower order mux, higher order mux can be designed. Here, 4x1 mux is designed using 2x1 mux. 

<img width="699" height="434" alt="image" src="https://github.com/user-attachments/assets/ebd8a05d-fde4-47c4-91b9-c4d06000f57c" />

Pulse signals are given as inputs to the 4x1 mux in the testbench circuit.

<img width="566" height="410" alt="image" src="https://github.com/user-attachments/assets/b5c70b6f-6367-4b1c-b3fb-d6c9ad6437b8" />

The operation of 4x1 mux can be observed from the output.

<img width="940" height="373" alt="image" src="https://github.com/user-attachments/assets/7f02fe02-4c71-468a-87c2-afecaaf6b1c7" />

3 to 8 DECODER

The 3 to 8 decoder is one that has 3 input lines and 8 (2^3) output lines. Based on the  3 bit input combination, either of the 8 outputs is set active high and the remaining outputs are active low. The truth table of 3 to 8 decoder is: 

<img width="466" height="353" alt="image" src="https://github.com/user-attachments/assets/8156acfa-bcca-4aa5-b224-61770357489c" />

Using this truth table, we can derive the Boolean expression for each output as follows –

<img width="408" height="372" alt="image" src="https://github.com/user-attachments/assets/ea7c79c0-abdf-4d82-bf12-e2a3f18e1b52" />

As we can see, each output term contains products of input variables, hence they can be designed with the help of AND gates. The schematic of 3 to 8 decoder implemented in Cadence Virtuoso is shown below:

<img width="578" height="632" alt="image" src="https://github.com/user-attachments/assets/fb4e5c2e-30c0-4042-8368-142f507057cc" />

Testbench circuit for the above schematic:

<img width="476" height="378" alt="image" src="https://github.com/user-attachments/assets/1f7099b9-b8ae-46bd-8f3b-e3610b94d556" />

Output obtained:

<img width="895" height="356" alt="image" src="https://github.com/user-attachments/assets/aedcfb42-cf64-46cc-a56f-a4dbbb4e68f2" />



