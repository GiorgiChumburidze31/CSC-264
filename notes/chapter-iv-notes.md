# MARIE: An Introduction to a Simple Computer

## MARIE 

A Machine Architecture that is Really Intuitive and Easy. 

Book uses `Intel` and `MIPS` machines, and the two popular architecrures relfecting these two are `RISC` and `CISC` architectures. 

**RISC:** Reduced Instruction Set Computer, focuses more on speed and efficiency during each instruction because each instruction takes `one clock cycle, per tick,` meaning that the instructions given are simple enough to process them extremely quickly.

> Simple and broken down code, more lines


**CISC:** Complex Instruction Set Computer, focuses more on compressed instructions in less lines, however these complex lines `take more clock cycles per tick.` 

> Complex code, more instructions in single line, less lines. 


## Memory 

Memory in a computer is like a giant filing cabinet. Computer stores **`instructions, and data`** in its memory, which then later is used by the **`CPU`**

Memory is stored in binary, 0, and 1, with its assigned address. 


## Types of Memory
Computer has three main types of memory 
#### Random Access Memory (RAM)
```sh
Memory here is not permenant and only gets stored temporarily inside RAM. In order to retain data from RAM it must be saved to a SSD/HDD to have it saved permanantely. 
```
Examples of Ram: 
* Typing Documents, gets stored in `RAM` 
* Playing Video Games (Failure to save from `RAM` = process lost)

### Read Only Memory (ROM)

**`Read Only Memory (ROM)`** is the kind of memory that retains only the essential data even after the computer is turned off. 

This `"essential data"` is used for booting, or `bootstrraping` up the computer. ROM contains `BIOS` which is Basic Input/Output System, and this is the first thing that runs when our computer turns on.  


### Bootstrapping 

The following process is how a computer becomes operational upon powering it on. 

#### Hardware Initilization

* Electricity is provided to all the major components, RAM, CPU, and Storage Drives. 

* At this point CPU is loaded, however it has no instructions to execute. 

#### CPUs' Exexution of Code in ROM 

* CPU has a small permanent memory chip called `ROM,` and it reads memory from it each time it is booted up. 

* It looks for BIOS or `UEFI (Unified Extensible Firmware Interface)` which is **`contained inside ROM`**
    * `BIOS/UEFI` checks the hardware, (Keyboard, RAM, Storage Devices, Computer Screen) and makes sure that everything works. This is also called `(POST) Power On Self Test`  

    * Then it looks for a bootable storage, and determines which storage device has a OS on it. 

#### Loading Bootloader from Storage

* After the BIOS finds the storage `containing OS`, then it moves on to loading `"bootloader" into memory`(a program, always gets loaded first)

* **`Finally`** Then Bootloader loads the Operating System or `the OS Kernel` (core part of OS) into the `RAM` (Since CPUs only work with RAM)

#### Operating System Takes Over

* Once the following process is done, OS takes over, and CPU begins to execute instrucions from RAM. 

* It also  initilizes interfaces, device drivers, and gives you control to the rest of the system. 


### Solid State Drive Memory / Hard Disk Drive (SSD/HDD) 


## CPU 

