# EXPERIMENT--01-ALP-FOR-8086
# Name :PRAVEEN RAJ.R
# Roll no : 212224230207
# Date of experiment : 29/08/2025





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


##TRUTH TABLE
<img width="1205" height="896" alt="image" src="https://github.com/user-attachments/assets/6e607707-425b-48a8-8e45-d689227d07a0" />




## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00H
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC LOOP1
INC CL
LOOP1: MOV [3005H],AX
MOV [3007H],CL
HLT
```



## Output  
 <img width="1920" height="1200" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/8bb714dd-4f5e-4a3b-b40f-fe5f25f7b4a1" />

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
LOOP1: MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
<img width="1920" height="1200" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/a897e71f-bb74-42c7-8d9a-e897d31b95f5" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
<img width="1919" height="1199" alt="Screenshot 2025-08-22 162007" src="https://github.com/user-attachments/assets/ad63fe38-5f26-4cce-98f8-c50789318a58" />



## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3011H],AX
MOV [3013H],DX
HLT
```
## Output  
<img width="1920" height="1200" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/5ca5c3c9-e7c3-4f68-8a58-b09f49866c88" />

## Programs for logical  operations
## And
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

## Output
<img width="1920" height="1200" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/97715abc-8653-4b46-9838-0f51116926d9" />


## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1920" height="1200" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/6ac14f40-177d-49da-ab3b-e7f5a74cf11b" />


## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1920" height="1200" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/95195e65-23f4-461f-9a7c-a12d2701897c" />

## NOT
```
MOV AX,[3001H]
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1920" height="1200" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/614da235-40ab-46c4-a91a-7d6e25906a43" />

## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX   
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1920" height="1200" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/5e588254-3c4a-41ac-8ce5-2806acab192f" />

##NOR
```
MOV AL, [3001H]  
OR AL, [3003H]  
NOT AL  
MOV [3011H], AL  
HLT  
```
## Output
<img width="1920" height="1200" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/607d6551-5dc7-4b53-923c-2971ee273566" />

## Result :
 
Thus, the Assembly Language Programs (ALP) for performing fundamental arithmetic operations (Addition, Subtraction, Multiplication, Division) and logical operations (AND, OR, XOR, NOT, XNOT) were written, executed successfully using the 8086 emulator, and the outputs were verified.







