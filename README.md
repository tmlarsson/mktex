# mktex
A script to compile latex documents using pdflatex and biber.

Usage.
To compile a document one must specify the filename of the given document. 
This is done by passing the filename, without the '.tex' ending after the '-f' flag.

If one want to compile using biber, simply pass along the '-b' flag.

If you want the script to remove all 'unnessesary' files that comes along with the compilation, pass along the '-c' flag.

Example usage:

mktex -f paper -b -c

which compiles a document called 'paper' 
