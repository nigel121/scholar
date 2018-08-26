TEX = pandoc details.yml more-details.md
src = template.tex
FLAGS = --pdf-engine=xelatex

resume.pdf : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm resume.pdf
