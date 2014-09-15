all: 3nodesIsMinimum.png
all: livering_observed.txt
all: livering_wiki.png
all: t1.png

%.png : %.txt
	neato -Tpng $< >$@
	open $@

clean:
	rm -f *.png
