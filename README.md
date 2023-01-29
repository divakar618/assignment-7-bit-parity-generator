# assignment-7-bit-parity-generator

TITLE : 7 Bit parity generator

AIM:To Design and Simulate 7 Bit parity generator using verilog code.

introduction :

The parity generator is a combination circuit at the transmitter, it takes an original message as input and generates the parity bit for that message and the transmitter in this generator transmits messages along with its parity bit.
yhe classification of this generator is

![WhatsApp Image 2023-01-29 at 13 21 15](https://user-images.githubusercontent.com/121932143/215315681-ebb4a7b8-0569-46ce-8ea3-431e389898cc.jpg)

The even parity generator maintains the binary data in even number of 1’s, for example, the data taken is in odd number of 1’s, this even parity generator is going to maintain the data as even number of 1’s by adding the extra 1 to the odd number of 1’s. This is also a combinational circuit whose output is dependent upon the given input data, which means the input data is binary data or binary code given for parity generator.
In odd parity bit, the code must be in an odd number of 1’s, for example, we are taking 5-bit code 100011, this code is said to be odd parity because there is three number of 1’s in the code which we have taken. In even parity bit the code must be in even number of 1’s, for example, we are taking 6-bit code 101101, this code is said to be even parity because there are four number of 1’s in the code which we have taken

logic diagram :

  ![image](https://user-images.githubusercontent.com/121932143/215315744-f2bd4034-d78c-4f90-88dd-52abf873be10.png)

Truth table :

   ![image](https://user-images.githubusercontent.com/121932143/215315931-6a1f8bdf-2211-4357-855c-d24d60d71571.png)
   
program :
 
module lg(a,b,c,d,e,f,g,h,pe);
input a,b,c,d,e,f,g,h;
output pe;
wire x,y,z,w,q,l,m;
xor(x,a,b);
xor(y,x,c);
xor(z,y,d);
xor(w,z,e);
xor(q,w,f);
xor(l,q,g);
xor(pe,l,h);
endmodule

RTL diagram :

![Screenshot (39)](https://user-images.githubusercontent.com/121932143/215316044-03750deb-bed7-4e51-b067-4cd35b261122.png)

Timing diagram :


![Screenshot (40)](https://user-images.githubusercontent.com/121932143/215316082-a5b40d27-fdba-427b-ac97-dfde6ea9f6c5.png)

Result :
    Thus the 7 Bit parity generator is verified.
