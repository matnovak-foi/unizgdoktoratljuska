U slučaju da studirate na foi i želite koristiti R za generiranje latex predloška pa onda dalje možete pronaći projekt: https://github.com/matnovak-foi/R_LaTeX_phdTemplateExample

## LaTeX ljuska za izradu doktorskog rada na Sveučilištu u Zagrebu.


* ljuska je (do na Arial font) prilagođena Dr.Sc.08 dokumentu
* primjerak radnje nalazi se u "doc" direktoriju.


Nekoliko natuknica (dok ne uhvatim vremena napisati malo bolju dokumentaciju)

* folder "bibliografija" zamišljen je za čuvanje .bib datoteka koje sadrže bibliografiju u BiBTeXu. 
* folder "doc" sadrži primjerak disertacije te će jednog dana sadržavati i dokumentaciju
* datoteka "documet.tex" je glavna (ishodišna) tex datoteka (NJU KOMPAJLIRATE!)
* folder "dodatno" sadrži dodatne postavke poput paketa, glossaryja, dodatnih komandi i environmenta
* folder "naslovnice" sadrži naslovnice. Potrebno je editirati naslov.tex i 
  prilagoditi odgovarajuće varijable. Nakon toga treba kompajlirati naslov.tex
* folder "ostalo" sadrži sažetak, zaključak i slično
* folder "poglavlja" sadrži poglavlja i odgovarajuća potpoglavlja
* folder "skripte" sadrži korisne \*nix skripte za prebacivanje između utf-ascii
  te hrvatske navodnike


**Kompajliranje**:
```
$ pdflatex document.tex
$ bibtex document.tex
$ pdflatex document.tex
$ pdflatex document.tex
# mozda i makeglossaries
```

Ako koristite linux onda je koristan alat 
[Latexmk](http://users.phys.psu.edu/~collins/software/latexmk-jcc/)
 (koristi datoteku latexmkrc) pa mozete zamijeniti prijašnje linije samo sa
```
$ latexmk -pdf document.tex
```
U slučaju da studirate na foi i želite koristiti R za generiranje latex predloška pa onda dalje možete pronaći projekt: https://github.com/matnovak-foi/R_LaTeX_phdTemplateExample 
