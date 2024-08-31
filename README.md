# EXPERIMENT--01-ALP-FOR-8086:

Name : Nemaleshwar H

Roll no :212223240142

Date of experiment : 31/08/2024

## Aim: 
To Write and execute ALP on fundamental arithmetic and logical operations:
## Components required: 8086  emulator:
## Theory:
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


## Running the Emulator:
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
3.	Write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 
4.	Compile the program and check for the errors 
5.	Run (once there is no syntax error) 
6.	Click OK to see/view the output of your program on the Emulator screen. 
7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table.


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)

9.	Click on emulate to start emulation 

![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)

10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 

![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic  operations:

## Addition  of 8 bit ALP:
```
org 100h  

mov al, 25h    
mov bl, 13h    
add al, bl     
mov [2375h], al

ret            
```
## OUTPUT: 
![alt text](359584864-9ea6d67d-0199-40bc-815e-a4feaab54ad3.png)

## Subtraction  of 8 bit numbers  ALP:
```
org 100h

mov al, 25h    
mov bl, 13h    
sub al, bl     
mov [0009h], al 

ret
```
## OUTPUT:

![sub](359584917-9c4316ab-c006-439e-bf19-330e6ee847fd.png)

## Multiplication Operation:
```
org 100h

mov ax, 4101h  
mov [6000h], ax
mov bx, 2218h  
mov ax, [6000h]
mul bx         

mov [5008h], ax


ret
```
## OUTPUT:

![alt text](359585155-c0319816-0d3a-4a0c-be51-14ffaf78f693.png)
## Division Operation:
```
org 100h            

mov ax, 0b161h      
mov dx, 0           

mov [2000h], 0a415h 
mov bx, [2000h]     
div bx              

mov [1121h], ax     

ret                 
```
## OUTPUT:
![div](359585424-631da9cc-78b9-4772-a950-b90492a880e7.png)
## LOGICAL OPERATIONS:
### OR Operation:
```
org 100h

mov ax, 0A23h
mov si, 0b13h
or ax, si


ret
```
### OUTPUT:

![or](359586099-85528a19-bee2-4cd8-bc4e-5cbf296714e7.png)
### AND Operation:
```
org 100h

mov di, 0532h 
mov cx, 0A23h
mov dx, 0b13h
and cx, dx   
mov [0007h], cx

ret
```
### OUTPUT:
![and](359586420-11e114c4-18f4-4e4c-b0da-559f7db33d69.png)
### NOT Operation:
```
org 100h

mov ax, 0A32h  
not ax         
               
mov [0008h], ax

ret
```
### OUTPUT:
![not](359587459-1a94e005-7542-4deb-8fc4-8a0d780613c2.png)

### XOR Operation:
```
org 100h
mov ax, 0A32h  
mov bx, 0B13h  
xor ax, bx     
               
mov [0028h], ax

ret
```
### OUTPUT:
![alt text](363272832-a9dc326c-c72b-4d25-930d-6956be9a421c.png)
## Result :
Thus, Assembly Language Program for fundamental arithmetic and logical operations are exected succesfully.






