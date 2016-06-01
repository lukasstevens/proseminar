TARGET=praesentation

.PHONY: all clean watch

OPTIONS=-bibtex -pdf -pdflatex="pdflatex --shell-escape"

all: $(TARGET).tex
	latexmk $(OPTIONS) $(TARGET).tex
force: $(TARGET).tex
	latexmk -gg $(OPTIONS) $(TARGET).tex
watch: $(TARGET).tex
	latexmk -pvc $(OPTIONS) $(TARGET).tex
clean:
	rm -rf *.nav *.snm *.vrb *.aux *.bbl *.blg *.fdb_latexmk *.fls *.lof *.log *.lot *.out *.gnuplot *.table *.toc
