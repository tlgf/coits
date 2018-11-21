all: presentation.pdf

presentation.pdf: presentation.tex
	pdflatex presentation.tex
	evince presentation.pdf &
force:
	pdflatex presentation.tex
	make read

read:
	evince presentation.pdf &

go:
	evince -s presentation.pdf

slides: presentation.pdf
	pdflatex -jobname=slides.tex presentation.tex
	evince slides.pdf
