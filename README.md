# 2c.py
python 2.7 to C compiler

This is a pre-release of a Python-to-C translator (under development from 2010 year).

It compiles Python 2.7 code to C code, thus allowing to translate a single Python module to a binary file .

Handles all the the language constructs.
 
Certainly there are some bugs.

Usage:

 
       python 2c.py [options] filename.py
 
Options:
  -h, --help             show this help message and exit
  -e, --build-executable build executable (not extension module)
  --show-debug           show compiler debug messages
  --no-line-numbers      supress line number code
  --added-pass-subscr    add pass to evaluate type indexing
  --use-gcc-extension    use gcc extension
  --no-generate-comments supress internal tree comment
  -c, --no-compile       only generate C-code, no compile
  -i, --indent           run 'indent' for generated C file
  --no-direct-call       supress direct C call convenction
  --decompiler-print     print decompilation psevdocode
  --optimiser-debug      trace C-code optimisation
  --no-optimiser         no text optimisation
  --inline-subst         inline subst of small's def
  -f OPT_FLAG, --compiler-flag=OPT_FLAG
  -n C_NAME, --c-named-as=C_NAME
  --use-cfunc            generate cfunc (obsolete)

       
After a successful compilation there would be a filename.dll or filename.so file in the site-packages directory, or 
executale code at current directory (with option -e )

Using the generated binary code gives a speed boost from 2 to 4.5 times ☺. 
 

 
