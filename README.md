# mktex
A script to simplify compilation of LaTeX documents in the terminal.

The script uses pdfLaTeX and biber to compile .tex documents.

Usage example: [possible flags]
  mktex filename [-b -c -m]
  
  options:
    -h, --help            show brief help
    -b, --biber           compile using biber
    -c, --clean           remove unnecessary files
    -m, --minted          Use this flag to use minted
    
The minted flag, '-m', is used due to a potential security risk of using the flag '-shell-escape' with pdfLaTeX. With '-shell-escape' packages can potentially get access to the terminal to execute commands. 

If you need a latex-template for a document such as a lab report. See @kwlg template over at https://github.com/kwlg/latex-template/.
