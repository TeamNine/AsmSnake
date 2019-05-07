# Asm:snake:
Small university project to improve assembler language knowledges and legacy boot steps.
It is well known snake game written on assembler language in order to be placed in the booting area (MBR)

In programm was used : 
- DOS text (03h - 80x25) and graphic (12h - 640X480 16bit) mode 
- read/write operation to load extra code in memory (more then 512 bytes)
- reboot command
- commands to check keyboard buffer for game manipulations
- timers (for random function and change speed of the game)

# Compile
Just run `compile.bat` [Nasm](https://www.nasm.us/) should be installed and added to PATH (or you can run `nasm -f bin -o boot.img snake.asm` from terminal).

# Launch
I use [Qemu](https://www.qemu.org/) as virtual machine, if you have it too, run `start.bat`
If you usse another VM, check documentation for your VM and start i386 machine with boot image that you got after compilation

# Demo
[![Alt text](https://img.youtube.com/vi/o3MWuYKmRg0/0.jpg)](https://www.youtube.com/watch?v=o3MWuYKmRg0)