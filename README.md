# Colossal Cave for VM/CMS

Important note: I didn't write this port of Colossal Cave.  I don't know
who did.  My only role here was rescuing it from the Internet Archive,
since it's no longer hosted at ua.edu, and then running it through some
converters to get files in a form that people without VM/CMS can easily
use.

Adam Thornton, 15 May 2016

## VMARC

The VMARC file was unpacked with Leland Lucius's VMA.
( http://www.homerow.net/zvm/vma/ )

## Conversion

The ASCII subdirectory contains the results of unpacking with ```vma
-a```.

EBCDIC is the native unpacking.

You can try this with iconv or dd, but the record length is tricky and
everything ends up on one big line unless you're really careful.  Using
```vma``` is a lot easier.

## Compilation

Not sure I've ever compiled anything for PL/I in VM/CMS, but assuming
you can get your hands on a compiler, the ASSEMBLE files clearly are
callable subroutines used by the main PL/I program.  RANDU.FORTRAN seems
to be a PRNG.

The project to build a PL/I front end to GCC apparently stalled out in
2007.

IBM will sell you a PL/I compiler, of course, but that probably does not
help.  And they don't sell it for Linux or VM/CMS.  You could get an AIX
60-day trial.

Iron Spring has a closed-source compiler for OS/2 and Linux (x86,
presumably), which appears to be free-to-use at least for now:
http://www.iron-spring.com/download.html

However, it's not at all clear you'd actually want to run this version;
it appears to be not significantly different from all the other
350-point Adventure versions out there.
