# EXPERIMENT--01-ALP-FOR-8086
# Name :PRAVEEN RAJ.R
# Roll no : 212224230207
# Date of experiment :29/8/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)


## TRUTH TABLE
<img width="933" height="695" alt="Screenshot 2025-08-29 161358" src="https://github.com/user-attachments/assets/a67a7891-4de5-49e9-9f8e-c4a0035ea612" />




## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
CL,00H
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC LOOP1
INC CL 
LOOP1:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  

 <img width="1920" height="1200" alt="Screenshot (156)" src="https://github.com/user-attachments/assets/14601cf8-5525-45be-b48f-613f6b67d8a4" />

## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00H
MOV AX,[3001H]
MOV BX,[3003H]   
SUB AX,BX
JNC LOOP1
INC CL   
NOT AX
INC AX
LOOP1:
MOV [3005H],AX
MOV [3007H],CL
HLT
 ```
## Output  
<img width="1920" height="1200" alt="Screenshot (157)" src="https://github.com/user-attachments/assets/c0298ff8-9e64-45cb-bbd0-93e3e57608ea" />


## Multiplication alp
```
MOV AX,[3001h]
MOV BX,[3003h]
MUL BX

MOV [3005h],AX
MOV [3007h],CL
HLT
```
 ## Output  
<img width="1920" height="1200" alt="Screenshot (158)" src="https://github.com/user-attachments/assets/ed2696ae-2d61-4cdb-8533-5f4a82104efc" />


## Division alp 
```
MOV AX,[3001h]
MOV BX,[3003h]
DIV BX
MOV [3005h],AX
MOV [3007h],DX
HLT
```
## Output  
<img width="1920" height="1200" alt="Screenshot (148)" src="https://github.com/user-attachments/assets/c1651dad-9c2a-4adf-b3a4-9c24d21737b2" />




## LOGICAL OPERATORS
## AND ALP
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1920" height="1200" alt="Screenshot (159)" src="https://github.com/user-attachments/assets/2fe345c4-b65a-4fc0-a282-b08828e527c7" />


## OR ALP
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1920" height="1200" alt="Screenshot (152)" src="https://github.com/user-attachments/assets/d9e16b99-f83c-4fa9-82f8-592f8162a68d" />



## NOT ALP
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT

```

## OUTPUT

<img width="1920" height="1200" alt="Screenshot (153)" src="https://github.com/user-attachments/assets/09fb95ae-41b1-423b-bfa3-044c2db644b3" />

## NOR ALP
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1920" height="1200" alt="Screenshot (151)" src="https://github.com/user-attachments/assets/518d267b-0258-49d6-824b-00914c6b6f53" />


## XOR ALP
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1200" alt="Screenshot (154)" src="https://github.com/user-attachments/assets/ffdc5a73-39e7-4660-bc03-5408695cec46" />

## XNOR ALP
```
MOV AX,[3001H]
MOV BX,[3006H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1200" alt="Screenshot (155)" src="https://github.com/user-attachments/assets/39dab9cc-ef0b-4354-b049-0e2584f14b8b" />


## Result :
 

Thus the execution of ALP on fundamental arithmetic and logical operation has been performed successfully






