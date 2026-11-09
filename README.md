# TheSquareLiminalChip
A custom devboard that can be a replacement for the ESP and Rasberries.

  <img width="382" height="577" alt="3Drenderweek5" src="https://github.com/user-attachments/assets/c56777d4-8b9d-4458-8abb-64b7746a13f2" />

# Description
This is a custom devboard meant to be like the ESPs and Rasberries. It has a USB-C port, flash memory, IOs, etc. Specifically this is a RP2040 devboard designed to be a versatile, low-cost microcontroller platform. Basically, I made my own microcontroller.
# Features
* USB-C Port
* I/O Headers
* RP2040 Rasberry Pi
* Flash Memory storage
* Crystal Oscillator

# BOM

|Item|Qty|Supplier|Cost|Link|
|-----|--|-------|-----|-----|
|Assembled Devboard|1|JLCPCB|$65.68|[Link](	https://jlcpcb.com/)|

# Schematic and PCB Design

<img width="916" height="634" alt="Screenshot 2026-11-08 at 6 22 35 PM" src="https://github.com/user-attachments/assets/2458d8d4-ba31-4c23-94c6-43a5bc940356" />

The schematic design for this board is pretty straight forward. The top image is the finished product, but I had to overcome some serious errors in routing to get to this point. I don't know when or how, but I somehow flipped or wired the wrong ports! 

<img width="400" height="300" alt="Screenshot 2026-11-07 at 4 48 04 PM" src="https://github.com/user-attachments/assets/9269d4b2-f495-49a5-b314-cb809d96dc24" />

<img width="400" height="300" alt="Screenshot 2026-11-07 at 4 54 36 PM" src="https://github.com/user-attachments/assets/122e1239-85cd-471c-bac1-d0fbacb617d9" />

These are the parts that I messed up, which affected the SMD pads on my PCB board, which was a PAIN IN THE SOUTH POLE. I had to spend time diving through my own mess to clean everything up and even then, the footprints were ALSO WRONG. The SMD pads for some parts where in totally wrong positions and I needed to use exact positioning to put them in their place. This also took a long time. 

Then, just when I thought I was finished by pressing DRC, I got like 38 errors, so I had to then spend time to troubleshoot everything until I was left with 5 errors.

<img width="982" height="508" alt="lasterrors" src="https://github.com/user-attachments/assets/f57f73c3-5ddf-4ded-8213-e881d9e4e387" />

These errors were relatively easy to fix, all I had to do was make the thermal relief spokes 1 instead of 2 and it solved all my problems!

# Assembly and Conclusion

Since I was a beginner, this project was mainly learning and troubleshooting, and I think the troubleshooting part is really important to project in general as I was actually learning on how to solve problems. NOW, I need to assemble this thing by soldering and it ain't gonna be easy. The board is SMALL, like the size of my palm, so that's gonna be fun.

