## File: Makefile

LATEST=SSAQLD_BranchCouncil_Oct2019_minutes

.PHONY: all
all: ${LATEST}.pdf

PANDOC = pandoc
PANDOC_OPTS = -s

 ## pandoc pattern rules 
%.pdf: %.md
	${PANDOC} ${PANDOC_OPTS} $< -o $@
%.docx: %.md
	${PANDOC} ${PANDOC_OPTS} $< -o $@
%.html: %.md
	${PANDOC} ${PANDOC_OPTS} $< -o $@
%.tex: %.md
	${PANDOC} ${PANDOC_OPTS} $< -o $@

## produce pdf, html, docx etc from test.Rmd
SSAQLD_BranchCouncil_Aug2019_minutes.pdf: ${@:.pdf=.md}
SSAQLD_BranchCouncil_Aug2019_minutes.docx: ${@:.pdf=.md}
