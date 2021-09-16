
all:
	latexmk -synctex=1 -interaction=nonstopmode -file-line-error -pdf -shell-escape -enable-write18 -recorder proj_records.tex
clean:
	rm -f `ls -p | grep -v "/\|proj_records.tex\|proj_records.pdf\|Makefile"`