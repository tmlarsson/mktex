# mktex
A script to simplify compilation of LaTeX documents in the terminal.

The script uses pdfLaTeX (and biber) to compile .tex documents (with references).

Usage example: [possible flags]<br />
  mktex filename [-b -c -m]
  
options: <br />
  -h, --help            show brief help<br />
  -b, --biber           compile using biber<br />
  -c, --clean           remove unnecessary files<br />
  -m, --minted          Use this flag to use minted<br />
  
The filename can have three formats:<br />
  'filename'<br />
  'filename.'<br />
  'filename.tex'<br />

The minted flag, '-m', is used due to a potential security risk of using the flag '-shell-escape' with pdfLaTeX. With '-shell-escape' packages can potentially get access to the terminal to execute commands. 

If you need a latex-template for a document such as a lab report. See @kwlg template over at https://github.com/kwlg/latex-template/.
