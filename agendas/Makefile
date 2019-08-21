## File: Makefile

.PHONY: all
all: SSAQLD_BranchCouncil_Aug2019_agenda.pdf

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
SSAQLD_BranchCouncil_Aug2019_agenda.pdf: ${@:.pdf=.md}
SSAQLD_BranchCouncil_Aug2019_agenda.docx: ${@:.pdf=.md}
