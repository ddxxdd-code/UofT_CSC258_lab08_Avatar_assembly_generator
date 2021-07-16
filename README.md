# UofT_CSC258_lab08_Avatar_assembly_generator
## CSC258 lab08 Avatar assembly generator
### Introduction
This is a generator for the task of writing MIPS assembly code to display an avatar of airplane on bitmap display on MARS simulator.
### How to run
Use the command to compile the file
```
gcc -o Avatar_assembly_generator Avatar_asm_gen.c
```
Then run
```
./Avatar_assembly_generator my_avatar.asm
```
This will create a file 'my_avatar.asm' at your current location which contains code in MIPS assembly can be used to display airplane on bitmap display.

### How to change the default avatar
Open the file Avatar_asm_gen.c.

Change color selection: in #define, you can change/add colors as you like and its definitions. (don't forget to change the part in "Write start and initialize the registers" where COLOR1, COLOR2, COLOR3, COLOR4, COLOR5 are used corresponding to your change of definition of macro and the part in the output string to match your design)

Change shape: change the shape of the avatar by changing the matrix canvas\[32]\[32]'s contents. In the matrix, 0 is for no color, 1, 2, 3, 4, 5... are for the colors you defined in order: COLOR1, COLOR2, COLOR3..., these are the colors of the units in the bitmap result.

### Display specifications

Unit Width in Pixeld: 8

Unit Height in Pixels: 8

Display Width in Pixels: 256

Display Height in Pixels: 256

Base address for display: 0x10008000($gp)

### Author

Dedong Xie

2021-07-16
