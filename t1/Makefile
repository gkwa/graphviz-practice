all: d1_d2_dot.png
all: 3nodesIsMinimum.png
all: livering_observed.png
all: livering_wiki.png
all: t1.png

# multiple using dot parent dotfile
d1_d2_dot.png: d1.png d2.png

# multiple using montage to combine multiple pngs
mm: d1_d2_montage.png
d1_d2_montage.png: d1.png
d1_d2_montage.png: d2.png
	montage -geometry +2+1 -tile 2x1 d1.png d2.png d1_d2_montage.png
	open $@

%.png : %.dot
	neato -Tpng $< >$@
	open $@

clean:
	rm -f *.png
