# mktex
A script to simplify compilation of LaTeX documents in the terminal.

The script uses lualatex or pdfLaTeX (and biber) to compile .tex documents (with references). By default lualatex is used.

Usage example: [possible flags]<br />
  mktex filename [-b -c -m]
  
options: <br />
  -h, --help            show brief help<br />
  -b, --biber           compile using biber<br />
  -c, --clean           remove unnecessary files<br />
  -m, --minted          Use this flag to use minted<br />
  --pdflatex            Overrides the default compiler<br />
  --tikz                Compile only TikZ picures in standalone mode<br />
  --update              Updates mktex into the newest found on github<br />
  --gettex              Fetches the latest latex-template from kwlg<br />
  
The filename can have three formats:<br />
  'filename'<br />
  'filename.'<br />
  'filename.tex'<br />

The minted flag, '-m', is used due to a potential security risk of using the flag '-shell-escape' with pdfLaTeX. With '-shell-escape' packages can potentially get access to the terminal to execute commands. 

The TikZ flag, --tikz, can be used if one only want to compile a part of your document, e.g. a picture. This is done with the documentclass \usepackage[tikz]{standalone}, tikz is used if the file will be a tikz picture. Perfect if you have to create beatuiful pictures for e.g. a powerpoint.

The --pdflatex flag overrides the defualt setting of pdflatex if by some reson one would want to user pdflatex over lualatex.

The --update flag updates the script to the newest version found here on github. Needs sudo to be able to place the new script in /usr/local/bin/. Please look through the code before use, such that you feel condifdent with it.

The --gettex flag fetches the newest latex-template from @kwlg. This removes the need to manually copy over a template from a folder on your pc. The latex-template fetched is the one found at @kwlg's github over at https://github.com/kwlg/latex-template/.
