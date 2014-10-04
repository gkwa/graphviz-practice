all: d1_d2.png
all: 3nodesIsMinimum.png
all: livering_observed.txt
all: livering_wiki.png
all: t1.png

multiple:
	dot -Tpng d1.dot >d1.png
	dot -Tpng d2.dot >d2.png
	dot -Tpng d1_d2.dot >d1_d2.png
	open d1_d2.png

%.png : %.txt
	neato -Tpng $< >$@
	open $@

clean:
	rm -f *.png
