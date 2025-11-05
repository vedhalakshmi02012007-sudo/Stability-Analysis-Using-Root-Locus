# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![WhatsApp Image 2025-11-05 at 08 14 09_9c620c40](https://github.com/user-attachments/assets/0756d476-8608-4275-8b1a-18f8318ab324)

![WhatsApp Image 2025-11-05 at 08 14 09_32536836](https://github.com/user-attachments/assets/f4516d92-ee99-41a0-972b-e486cafa3423)

![WhatsApp Image 2025-11-05 at 08 14 10_2225303f](https://github.com/user-attachments/assets/7cb2b985-82ae-4824-8c98-3aebbf42eacd)

![WhatsApp Image 2025-11-05 at 08 14 10_e6707297](https://github.com/user-attachments/assets/f50fcf2e-f805-4407-ab36-892a90aa28f7)

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
num = [1];
der = [1 15 50 0];
sys =  tf(num,der);
rlocus(sys);
[k poles] = rlocfind(sys);

## output:
<img width="1920" height="1140" alt="Screenshot 2025-11-03 094615" src="https://github.com/user-attachments/assets/4f0b9782-8c39-48d8-b952-45eb6e3ed784" />

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is K < 743.7357
