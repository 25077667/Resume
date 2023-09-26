.PHONY: all clean

TEX = latexmk
RESUME_DIR = src
RESUME_SRCS = $(shell find $(RESUME_DIR) -name '*.tex')
BUILD_DIR = ./build
OUT ?= resume.pdf

all: $(OUT)
	cp -f build/$< .

$(OUT): resume.tex $(RESUME_SRCS)
	$(TEX) -xelatex -output-directory=$(BUILD_DIR) $<

clean:
	$(RM) -r $(BUILD_DIR)
