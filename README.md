## Titlesec, Titletoc, Titleps

This directory holds 3 packages for sectioning titles -- when used as
such (titlesec), in headers and footers (titleps) and in tables of
contents (titletoc).  They can be used separately, but you will get
most of them when used together.

### Titlesec

Sectioning titles, including margin and `wrap` titles, different
format in odd and even pages, rules above and below the title, 
adding new sectioning levels, measuring the width of the title, etc.

### Titletoc

TOC entries, with the possibility of changing the format in the middle
of a document, grouping the entries in a single paragraph, pretty
free-forms entries, partial tocs, etc. It's described in
`titlesec.pdf`.

### Titleps

Page styles with working top marks, access to top, first and bot marks
in a single header/footer, rules, headers/footers for specific floats
(kinda `\thispagestyle`), multiple sets of marks, etc.  An one-stage
mechanims is used, without intermediate `\leftmark`s or `\rightmark`s.

### Latest changes

```
2.13  2019-10-16
      - \markboth (which has been redefined in the LaTeX kernel) works
        again.

2.12  2019-09-09
      - Fix - Partial TOCs were severely broken.
      - Fix - An undefined section doesn't raise an error any more.

2.11  2019-07-16
      - New license: MIT.
      - Option nostruts, to remove struts inserted by titlesec.
      - Reorganized code: only sty files, removed def and tss ones
        (although the mechanism for tss still works).
      - Fix - Wrong hyperlinks in table of contents with the starred
        versions, because of a change of behavior of hyperref (it
        patches the behaviour of an internal macro in hyperref).
      - Fix - Wrong spacing with titleps and displayed text after a
        section.
      - Fix - Newly defined floats raised an error with titletoc.
```

### Installation

No .ins/.dtx preinstalation is required.  Move the files to a place 
where LaTeX can find them and typeset titlesec.tex.  All of files in 
this directory are necessary for titlesec.sty to work, except the 
manual titlesec.tex (and this 'readme' file). The manual requires
titlesec.sty and titletoc.sty.

Further details are available on

   http://www.texnia.com/titlesec.html

### Contact

Please, for suggestions, bug reports, etc., go to
More
   http://www.texnia.com/contact.html
