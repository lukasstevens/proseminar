BUILD_DIR=build
TARGET=ausarbeitung

.PHONY: all clean watch

OPTIONS=-gg -bibtex -auxdir=$(BUILD_DIR) -outdir=$(BUILD_DIR) -pdf

all:
	latexmk $(OPTIONS) $(TARGET).tex && cp $(BUILD_DIR)/$(TARGET).pdf .
watch:
	latexmk -pvc $(OPTIONS) $(TARGET).tex
clean:
	rm -rf $(BUILD_DIR)/*
