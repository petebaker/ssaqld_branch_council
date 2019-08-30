## File: Makefile

.PHONY: all
all: SSAQLD_BranchCouncil_Agenda_20190903.pdf

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
## although you can of course just use
## $ make any_filename.pdf   etc
SSAQLD_BranchCouncil_Agenda_20190820.pdf: ${@:.pdf=.md}
SSAQLD_BranchCouncil_Agenda_20190820.docx: ${@:.pdf=.md}
SSAQLD_BranchCouncil_Agenda_20190903.pdf: ${@:.pdf=.md}
SSAQLD_BranchCouncil_Agenda_20190903.docx: ${@:.pdf=.md}
