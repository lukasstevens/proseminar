BUILD_DIR=build
TARGET=ausarbeitung

.PHONY: all clean watch

OPTIONS=-bibtex -pdf -pdflatex="pdflatex --shell-escape"

all:
	latexmk $(OPTIONS) $(TARGET).tex
watch:
	latexmk -pvc $(OPTIONS) $(TARGET).tex
clean:
	rm -rf $(BUILD_DIR)/*
