# EXPERIMENT--01-ALP-FOR-8086

Name : LATHIKESHWARAN J

Roll no : 212222230072 

Date of experiment : 27/09/2024





## Aim:
To Write and execute ALP on fundamental arithmetic and logical operations
## Components required:
8086  emulator 
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







## Addition
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT    
          
```


## Output  
<img width="1920" height="1080" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/2f22746e-e45b-45b0-9867-a8823a5ca75c" />

## Subtraction
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
<img width="1380" height="747" alt="image" src="https://github.com/user-attachments/assets/6cec46a8-cc68-4564-8785-5afd5177f0a0" />


## Multiplication
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT 
```
## Output  
<img width="1255" height="930" alt="image" src="https://github.com/user-attachments/assets/fbb38c2f-d07d-4506-8e53-715887ffc08d" />

## Division
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT

```

## Output
<img width="1610" height="763" alt="image" src="https://github.com/user-attachments/assets/b1e4ca81-f14f-41ab-a4d6-1c5a278aaf24" />


## AND Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT

```

## Output
<img width="1586" height="757" alt="image" src="https://github.com/user-attachments/assets/06ddd782-05fd-4d08-a937-1e603dac7b8b" />


## OR Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT

```

## Output
<img width="1509" height="779" alt="image" src="https://github.com/user-attachments/assets/bf9e3d58-4bc0-430a-855a-5a2a7eab113f" />


## NAND Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## Output
<img width="1673" height="765" alt="image" src="https://github.com/user-attachments/assets/3e1dd32e-7499-48c2-a988-d36e09e13f0e" />


## NOR Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1340" height="759" alt="image" src="https://github.com/user-attachments/assets/cefab3d1-e970-4df4-a1f3-4997c91fcf9b" />



## NOT Operation
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## Output
<img width="1652" height="770" alt="image" src="https://github.com/user-attachments/assets/d3f6dc7b-8ba2-47bc-8390-b74f3fe30cf9" />



## XOR Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT

```

## Output
<img width="1582" height="764" alt="image" src="https://github.com/user-attachments/assets/0a9ef384-1281-4eb3-89ed-2fbe66d01db1" />


## XNOR Operation
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## Output
<img width="1519" height="769" alt="image" src="https://github.com/user-attachments/assets/d528111d-fe08-499a-9f0d-917489221079" />



## Result :
 
Therefore the program is successfully executed.







