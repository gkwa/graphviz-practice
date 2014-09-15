all: 3nodesIsMinimum.png
all: wiki.png
all: t1.png

%.png : %.txt
	neato -Tpng $< >$@
	open $@

clean:
	rm -f *.png
