.PHONY: preview spell clean

build/informe.pdf: informe.tex build
	pdflatex --output-directory build informe.tex
	pdflatex --output-directory build informe.tex
	pdflatex --output-directory build informe.tex

build:
	mkdir -p build

preview: build/informe.pdf
	evince build/informe.pdf &

spell:
	aspell -t check informe.tex -d es

clean:
	rm -rf build
