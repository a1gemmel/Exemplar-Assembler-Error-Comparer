Property of Andrew Gemmel

Made for use for CS241.

This script makes testing less of a hassle, works similar to runSuite from CS246. It must be used in the school linux environment in order to access cs241.binasm

NOTE: Not entirely useful for testing invalid input

Usage:
Create a text file with the names of all the .asm files you want to test (with the .asm)

Ex:

tests.txt
----------------------
loop.asm
max.asm
a1p3.asm
----------------------

Example script calls:

./testasm asm.rkt tests.txt

./testasm asm.cc tests.txt

./testasm asm.c tests.txt


The script will produce .out and .expect files that contain the xxd output of your assembler and cs241.binasm respectively. STDERR from your assembler will be redirected to a .error file.

Additionally, it will produce the result of comparing these files using cmp.

If no errors are found, there will be no output :)
