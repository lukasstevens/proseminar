BUILD_DIR=build
TARGET=ausarbeitung

.PHONY: all clean

all:
	latexmk -gg -bibtex -auxdir=$(BUILD_DIR) -outdir=$(BUILD_DIR) -pdf $(TARGET).tex && cp $(BUILD_DIR)/$(TARGET).pdf .
clean:
	rm -rf $(BUILD_DIR)/*
