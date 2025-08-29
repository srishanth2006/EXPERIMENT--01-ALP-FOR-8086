# EXPERIMENT--01-ALP-FOR-8086
Name : SRISHANTH J

Roll no : 212223240160

Date of experiment : 29-08-25


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







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```


## Output  
 <img width="1919" height="1190" alt="Screenshot 2025-08-22 154512" src="https://github.com/user-attachments/assets/220d379e-29f7-4ae1-aafc-a425d8c25d02" />

## Subtraction   of 8 bit numbers  ALP 
 ```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
<img width="1919" height="1199" alt="Screenshot 2025-08-22 160632" src="https://github.com/user-attachments/assets/97361b9f-d32e-49d2-8dcf-8befd3683357" />

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

<img width="1919" height="1199" alt="Screenshot 2025-08-22 162058" src="https://github.com/user-attachments/assets/7301158b-29f9-4ac4-acde-d9d83e54828c" />

## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  

<img width="1919" height="1199" alt="Screenshot 2025-08-22 162633" src="https://github.com/user-attachments/assets/93278765-6b88-4205-8d5b-9b18b46772aa" />

## LOGICAL OPERATIONS
## TRUTH TABLE
<img width="1957" height="1717" alt="image" src="https://github.com/user-attachments/assets/d2c3a2bf-14cf-4446-997a-e2060c2a3b63" />
## LOGICAL AND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/63098ce0-029f-4655-8e33-ccea0d679a7b" />

## LOGICAL OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="2559" height="1570" alt="image" src="https://github.com/user-attachments/assets/3b07b11d-54c8-4cba-be63-63354b986c6c" />

## LOGICAL NAND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/177d315d-a9ac-49a9-ae85-0d10cdaffaa8" />

## LOGICAL NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="2559" height="1596" alt="image" src="https://github.com/user-attachments/assets/373bb19b-486d-49de-9b65-81af7ed4914c" />

## LOGICAL NOT
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="2544" height="1599" alt="image" src="https://github.com/user-attachments/assets/5de76117-9e93-4843-b775-878dec5dc66e" />

# LOGICAL XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/7583e1f4-3ab6-4334-aca8-5fd395586b7e" />

## LOGICAL XNOR

```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/b2146e00-abb2-4f3f-ba70-5c9fda795109" />

## Result :
 Thus to Write and execute ALP on fundamental arithmetic and logical operations has been executed successfully.








