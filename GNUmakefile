.PHONY: all
all: $(patsubst %.txt,%.html,$(wildcard *.txt))
.PHONY: clean
clean:
	rm -f *.html

%.html: %.txt
	asciidoc  $<

.PHONY: git
git:		
	git add *.txt *.html
	git commit -e
	git push --force -u origin master

