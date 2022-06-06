.PHONY: src all clean

CC = latexmk
RESUME_DIR = src
RESUME_SRCS = $(shell find $(RESUME_DIR) -name '*.tex')
BUILD_DIR = ./build
TEMPLATE = awesome-cv.cls

all: resume.pdf
	cp build/$< .

resume.pdf: resume.tex $(RESUME_SRCS) $(TEMPLATE)
	$(CC) -xelatex -output-directory=$(BUILD_DIR) $<

clean:
	$(RM) -r $(BUILD_DIR)
