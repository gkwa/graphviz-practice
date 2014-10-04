all: d1_d2.png
all: 3nodesIsMinimum.png
all: livering_observed.png
all: livering_wiki.png
all: t1.png

d1_d2.png: d1.png d2.png

%.png : %.dot
	neato -Tpng $< >$@
	open $@

clean:
	rm -f *.png
