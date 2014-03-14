FILENAME=learn-you-a-scala
OUTPUT_DIR=output
PANDOC=pandoc
EXTENSIONS=markdown+yaml_metadata_block
PANDOC_FLAGS=-s -S -r $(EXTENSIONS) --filter pandoc-citeproc --csl=rose-school.csl
FILES=en/metadata.yaml en/chapter-01/index.md

$(shell [ -d "$(OUTPUT_DIR)" ] || mkdir -p $(OUTPUT_DIR))

all: epub html

clean:
	rm -rf output/*

epub:
	$(PANDOC) $(PANDOC_FLAGS) $(FILES) -o $(OUTPUT_DIR)/$(FILENAME).epub

html:
	$(PANDOC) $(PANDOC_FLAGS) $(FILES) -o $(OUTPUT_DIR)/$(FILENAME).html
