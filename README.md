80mm thermal printer driver tested and powered by Runelab S.R.L
=====

to make the printer work install the normal drivers from producer website, after this compile those repo using the command

make -f Makefile --> this command will compile the c custom drivers compatible with ARM (so Rasberry PI and similars)

after that lunch as root the command

sudo ./install --> this command will replace the old drivers with the new custom ARM drivers but leaving all the others settings as before

for any info or help contact me at marcobert37@gmail.com

----------------------------------------------------------------------------------------------------------

CUPS filter for thermal printer Excelvan ZJ-8001 and VT-8330

it's a modified version of klirichek's ZJ-58 cups for a 80mm thermal printer

We have worked with @redfish4ktc on this and we have been able to make the zj-80 printer work by modifying the rastertozj.c driver
The value has been modified on line 260.

Update: Add support to ARM architecture.
