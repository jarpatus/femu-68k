femu - A FPU emulator for classic Amigas
========================================
This program implements a custom exception handler for F-line exceptions.
The handler will then implement missing FPU instructions by sofware - hence 
this program can be considered to be a FPU emulator. 

Femu targets to 68040 and 6888x compatibility so actually femu is more powerful
than either one alone. However, femu uses internally double precision math so 
it's less precise than real FPU.

Femu should work with 020, 030 and 040 having no FPU. At the moment 060 is not 
supported, sorry!

Please also notice that this program is in alpha state and lot's of things are 
still missing, buggy or outright wrong. You are welcome to contribute of course!


Author
======
Jari Eskelinen <jari.eskelinen@iki.fi>


Thanks
======
Whole Apollo-Core team for asm help and testing efforts and support!


Compile
=======
You need make, vasmm68k and vlink for compile. Run "make clean" and "make" to compile femu.


History
=======
Femu was started by me (Jari Eskelinen) in order to learn some asm coding for fun. Since 
I had Vampire V2 which back then did not have FPU I decided to attempt to write a FPU emu
and I succeeded to some extent.

Femu was then used by Apollo team to develope hybrid soft/hard FPU for Vampire V2. Vampire
then outgrew femu and femu is no longer needed for Vampire V2; however, femu works with
old classic Amigas and could offer some fun with them even though performance will not be
great. 
