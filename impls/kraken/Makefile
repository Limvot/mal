STEPS = step0_repl

all: $(STEPS)

dist: mal

mal: stepA_mal
	cp $< $@

%: %.krak
	~/kraken/kraken $*.krak
	rm $*.krak.c

.PHONY: clean

clean:
	rm -f $(STEPS)
	rm -f mal
