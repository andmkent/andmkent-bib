(forked and modified from samth/gradual-typing-bib)

For papers written in [Scribble](http://docs.racket-lang.org/scribble/), this
bibliography can be installed as a package and referenced directly from the
paper. Use the following command to install:

`raco pkg install git://github.com/andmkent/andmkent-bib`

Sample use:

````
#lang scribble/base

@(require andmkent-bib
          scriblib/autobib)

@(define-cite ~cite citet generate-bibliography)

Original gradual typing papers
@~cite[st-sfp-2006 thf-dls-2006 mf-toplas-2007 gktff-sfp-2006].

@generate-bibliography[]
````
