.PHONY: all
all: $(patsubst %.txt,%.html,$(wildcard *.txt))
.PHONY: clean
clean:
	rm -f *.html

%.html: %.txt
	asciidoc  $<

.PHONY: git
git:		
	git add .
	git commit -m "$t" -m "$b"
	git push --force -u origin master

