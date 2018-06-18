PDF = mizosoji_orei.pdf atago_ofuda.pdf
DVI = mizosoji_orei.dvi atago_ofuda.dvi

.SUFFIXES: .tex .dvi .pdf
.PHONY: all clean

all: $(PDF)

.dvi.pdf:
	dvipdfmx -p "210mm,297mm" $<

.tex.dvi:
	platex $<

mizosoji_orei.pdf: mizosoji_orei.dvi

mizosoji_orei.dvi: mizosoji_orei.tex circular.sty

atago_ofuda.pdf: atago_ofuda.dvi

atago_ofuda.dvi: atago_ofuda.tex circular.sty

clean:
	rm -f $(DVI) $(PDF) *.aux *.log
