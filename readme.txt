o 1.0
-----

o is a routine to output a double number on the screen (in the terminal) to save bytes of codespace that would be required for a complete printf()- call.

The design of "o" is:

  #include <stdio.h>
  void o(double p)
  {printf(">%lf\n", p);}

To further save bytes for the codespace, also the #include<>- directive for including  stdio.h  is placed here.

So, in your program you just need to include o.cpp with

  #include "o.cpp"
  
(OK, with saves just 2 Bytes compared to stdio.h, but at least these)

Then output a number with

  o(number);
  
Where  number  can be a value or a variable in double- format.

This call indeed saves 15 bytes of code space.


Version history
---------------

Version 1.0

Initial version

