# ===== Usage ================================================================
#
# NOTE:
#   When running these commands at the command line, replace $(TARGET) with
#   the actual value of the TARGET variable.
#
#
# make                  Compile all *.md files to PDFs
# make <filename>.pdf   Compile <filename>.md to a PDF
# make <filename>.tex   Generate the intermediate LaTeX for <filename>.md
#
#
# make clean            Get rid of all generated files
#
# ============================================================================

LATEX_FLAGS = --toc --pdf-engine=xelatex --verbose --listings --top-level-division=chapter --toc --number-sections --columns=4
EXTRA_FLAGS = -f markdown+grid_tables+table_captions+blank_before_blockquote+pipe_tables+backtick_code_blocks+smart
AN_FLAGS = --variable=applicationnote
PANDOC = pandoc
MKDOCS2PANDOC = mkdocs2pandoc
DOC_TEMPLATE_PATH = ../doc_template
ARTICLE_TEMPLATE = $(DOC_TEMPLATE_PATH)/yml.tex
MD_TEMPLATE = $(DOC_TEMPLATE_PATH)/md.tex
YML_TEMPLATE = $(DOC_TEMPLATE_PATH)/yml.tex
BUILD_DIR = build

all:remove_all_pdf \
	$(BUILD_DIR)/ART_Pi_Smart_User_Manual.pdf 

remove_all_pdf:
	rm -rf $(BUILD_DIR) \
	rm -f $(BUILD_DIR)/*.pd $(BUILD_DIR)/*.tex

$(BUILD_DIR)/ART_Pi_Smart_User_Manual.pdf: index.yml
	mkdir $(BUILD_DIR)
	cp $(DOC_TEMPLATE_PATH)/* $(BUILD_DIR)/
	$(MKDOCS2PANDOC) -f $^ > $(BUILD_DIR)/temp.pd
	$(PANDOC) $(LATEX_FLAGS) $(EXTRA_FLAGS) --template=$(YML_TEMPLATE) -o $@ $(BUILD_DIR)/temp.pd
	$(PANDOC) $(LATEX_FLAGS) $(EXTRA_FLAGS) --template=$(YML_TEMPLATE) -o  $(BUILD_DIR)/temp.tex $(BUILD_DIR)/temp.pd 

	rm -f $(BUILD_DIR)/*.pd $(BUILD_DIR)/*.tex $(BUILD_DIR)/*.png

clean:
	rm -f $(BUILD_DIR)/* $(MAUNUL_DIR)/*.pdf *.aux *.log *.nav *.out *.snm *.toc *.vrb *.tex *.pdf *.pd  || true

.PHONY: all clean
