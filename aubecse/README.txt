INSTRUCTIONS

1. In the ./Chapter folder, copy the chapters.  Remove "\label{Chaptername} \lhead{Chapter x. \emph{CHAPTERNAME}}" in each file.
2. In the ./Appendices folder, remove "\label{Appendix} \lhead{Appendix x. \emph{APPENDIXNAME}}" in each file.
3. In bethesis.tex, 
	a. Specify your project tilte in \settitle{your project title}
	b. Specify number of authors in \setnauthor{n}
	c. Specify your names and rollnumbers  in \setauthorone{name}{num}, \setauthortwo{name}{num}, \setauthorthree{name}{num} -- as many as needed.
	d. Specify your guide name and designation in \setguide{guide's name}{guide's designation}

4. Front matter
	a. Edit your abstract in ./FrontMatter/abstract.tex
	b. Edit your acknowledgements in ./FrontMatter/ack.tex

5. Add your citations in bethesis.bib

6. Add your acronyms in the ./FrontMatter/acronyms.tex file. Specify the longest acronym as parameter in \listofacronyms[longest acronym].

TO COMPILE LATEX
Linux
In the terminal, run:
	$ pdflatex bethesis.tex
	$ bibtex bethesis
	$ pdflatex bethesis.tex # needed only if citations in bethesis.tex or bethesis.bib is changed
	$ pdflatex bethesis.tex

In case of changes in main content only
	$ pdflatex bethesis.tex  # should suffice

Windows
Should be pretty much the same

For acronyms, check ftp://ftp.tex.ac.uk/tex-archive/macros/latex/contrib/acronym/acronym.pdf
http://en.wikibooks.org/wiki/LaTeX/ covers most things you'll need to work with LaTeX

