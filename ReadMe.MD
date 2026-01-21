This project is my Learning C++ attempt. I really want to learn, but get bored with online courses. 
The plan thus far is to connect up to 16 Pico 2's to act as a unified computing cluster. 
It would function as a desktop, but all core processes would be split between each pico 2, 
possibly a stronger microcontroller for a graphics card, and a Raspberry pi 5 that would boot up in 
kiosk mode if the browser is selected, and shut down if the browser is closed. 

My Current plan for each Pico is (Not accounting for interfacing issues):

Pico 1: Director/ Powermanagement Pico (Tell's each Pico when a memory line is free for transfer and will cut power to Pico's not needed for current task)

Pico 2: I/O (Human Interfacing layer for keyboard, Mouse, and Track point. Other peripherals if necessary.)

Pico 3: Filesystem (Managing files on sd card and sending it to the necessary microcontroller)

Pico 4: Window System (Similar to X, Basically each Program Pico sends what to display in a window and programs are indexed in the Filesystem Pico)

Pico 5: Program Organizer Pico (Directs a program opened through the window manager as to which Program Pico to run on. Hopefully will make developing additional programs easier.)

Pico 6: Program Math Pico (Executes any math that a program may need such as spreadsheets)

Pico 7: Program Process 1 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 8: Program Process 2 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 9: Program Process 3 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 10: Program Process 4 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 11: Program Process 5 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 12: Program Process 6 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 13: Program Process 7 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 14: Program Process 8 (Copys a program from the file system, and executes and outputs it to the Window System Pico.)

Pico 15: Wireless Pico 9 (Wireless from a Pico 2 W to allow for internet applications such as Email. Would send internet data to a running Program Process that requested it.)

Pico 16: Sound Chip (Might be an Extra Program Process, and Sound generated on a different Chip)

Video Output Microcontroller (preferably something low power and atleast 8bit)

Raspberry Pi 5 (Browsing and Higher Power level programs)

