DOC=cv-complete
FINAL_NAME="resume thomas kappler"
LATEX=xelatex
BIBTEX=bibtex
PHOTODIR=/Users/thomas/Documents/Bewerbungen/CV/Bilder/
SCANSDIR=/Users/thomas/Documents/Bewerbungen/CV/Scans/
TEXINPUTS := ${TEXINPUTS}:$(PHOTODIR):$(SCANSDIR)

all: doc rename show

doc: $(DOC).tex
	$(LATEX) $(DOC).tex
	$(LATEX) $(DOC).tex

clean:
	rm -f *.aux $(DOC).blg $(DOC).bbl $(DOC).out $(DOC).lof $(DOC).toc $(DOC).brf *.log $(DOC).haux $(DOC).hlog $(DOC).lol $(DOC).lot

reallyclean: clean
	rm -f *~ $(DOC).pdf

rename:
	mv $(DOC).pdf $(FINAL_NAME).pdf

show:
	gnome-open $(FINAL_NAME).pdf &


FORCE:
