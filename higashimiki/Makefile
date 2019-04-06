PDF = mizosoji_orei.pdf atago_ofuda.pdf hancho_mtg6.pdf hancho_mtg7.pdf atago_orei.pdf general_assembly.pdf
DVI = mizosoji_orei.dvi atago_ofuda.dvi atago_orei.dvi

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

hancho_mtg2.pdf: hancho_mtg2.dvi

hancho_mtg2.dvi: hancho_mtg2.tex circular.sty


clean:
	rm -f $(DVI) $(PDF) *.aux *.log
