# imclean
IRAF Script for interactive corrections to Spitzer/IRAC images

Joseph L. Hora
May 2021

See the pdf manual file for more details on installing and running imclean.

Before running, edit the initclean.cl , imclean.cl, and spotclean.cl files to
point to the directory that you have placed these scripts in.


The ./src directory contains the c program source files, the ./bin directory
contains these programs compiled on a linux (CentOS) 64-bit Intel system. The
manual contains information on how to recompile these if needed.
There is a script in the src directory called "compile_imclean.sh" that will
compile all of the programs and move them to the ../bin directory.

