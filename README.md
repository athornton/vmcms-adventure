# Colossal Cave for VM/CMS

## VMARC

The VMARC file was unpacked with Leland Lucius's VMA.

## Conversion

ASCII-dd contains the results of EBCDIC-ASCII conversion with "dd", and
ASCII-iconv contains the results of EBCDIC-ASCII conversion with
"iconv", using EBCDIC-INT as the character set and using -c to skip
untranslatable characters.  You will notice this breaks the formatting
of the cave data (the first broken character appears to be a square
bracket from the "[sic]" after "fee fie foe foo").  The "text", and
"txtlib" files are assembler output anyway, so don't worry that they are
gibberish.

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
