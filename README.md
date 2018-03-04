This is fork of WinGup from gup4win/wingup
-----------------

from Don HO from notepad++ [`gup4win/wingup`](https://github.com/gup4win/wingup)


I made the following changes:
-----------------

to make it useful for .Net applications (for example for a Wpf-program) it is not possible to close the window by the 
Window Class to run the downloaded setup. Instead one option would be to close the application via the text in the 
title bar.
These changes have been made and all changes have been marked by me in the source code.
And I added a VS 2017 .sln solution.
Otherwise, the program works as described by Don HO. 



How to build it?
----------------

 0. You have to build cURL before building WinGup:
 ```
    a. Open VS2015 Native Tool Command for 32/64 bits
    b. go to curl winbuild directory:
       cd <your wingup source path>\curl\winbuild
	c. compile cURL by using one of the following commands, according the mode and archetecture of wingup you want to build.
       x64 release: nmake /f Makefile.vc mode=dll vc=14 RTLIBCFG=static MACHINE=x64
       x64 debug: nmake /f Makefile.vc mode=dll vc=14 RTLIBCFG=static DEBUG=yes MACHINE=x64
       x86 release: nmake /f Makefile.vc mode=dll vc=14 RTLIBCFG=static MACHINE=x86
       x86 debug: nmake /f Makefile.vc mode=dll vc=14 RTLIBCFG=static DEBUG=yes MACHINE=x86
```
 1. Open vcproj\GUP.sln
 
 2. Build WinGup with VS2017



To whom should you say "thank you"?
-----------------------------------

Don HO for the main work
<don.h@free.fr>
