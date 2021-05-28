# imclean
Script for interactive corrections to Spitzer/IRAC images

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


Below are the command instructions that print when starting up imclean:


Type a character listed below to perform an action.  Two are required to
specify an area on image.
The first letter usually specifies the first position, the second letter
defines the second position and the action. It is best to type the same
letter both times, to avoid confusion.
See the documentation for more description of each command.


c - column pulldown correction, whole column
l - column pulldown correction, specified area
r - row pulldown correction, whole row
k - row pulldown correction, specified area
d – row banding correction, whole row, only those > 0.5 sigma from median
D – row banding correction, whole row, force all columns to median
m – column banding correction, whole column, only those > 0.5 sigma from median
M – column banding correction, whole column, force all columns to median
v - banding correction for columns in specified region, only those > 0.5 sigma    
    from median
V - banding correction for columns in specified region, force all columns to median
w – warm mission pulldown corrector
a - mask the pixels in the rectangular region (no display refresh)
b - muxbleed correction, row following position
B - muxbleed correction, fix all 4 amplifiers
s - Stripe cleaning
S – Stripe cleaning, selected rows
p – fill selected pixels with interpolated values determined in same row outside of selected region (no display refresh)
P – same as “p”, except refresh display 
n - done editing, go back to mosaic
N - done editing, go to next file in list
u - undo previous edit on this image
U - undo all edits on this image
o - copy original bcd from directory specified on command line, overwrite current file
q - quit imclean


