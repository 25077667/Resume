
all:
	latexmk -synctex=1 -interaction=nonstopmode -file-line-error -pdf -shell-escape -enable-write18 -recorder Readme.tex
clean:
	rm -f `ls -p | grep -v "/\|cv.tex\|cv.pdf\|Makefile"`