LatexTemplate
=============

Default personal settings that I use while writing in latex.

_______________________________________________________________________
This project is to be included in a latex project. 

It has the most common libraries and definitions that 
I use and that not conlfict with many other things. 

The goal of this project is to offer a quick setup for starting a new latex project. I have
took in consideration my 5 years using latex, and all the stuff that I need to define over and over.
It it fits your needs, be my guest and make use of it. Unfortunately all of this kind of projects
leave the user with less customization capabilities. But I think that new users would find it
helpful to avoid all the ceremony required to start a latex project. 

(First compiling will return no errors, no bad boxes, no warnings, it is up to you
to keep it that way).


## Dependencies

- `texlive-fontextra`
- `texlive-latexextra`

## SETUP
Suppose you are planing to make a project ``myProject''.

Include the Template directory in your main project dierctory.

Make a file named myProject.tex in your main directory that contains only the line

```
\input{Template/main.tex}
```

Make a file named document.tex in your main directory also. Here you will put anything
you want your file to contain. Avoiding definitions, packages, indexing settings.
Your pure text content will be here.

This is an example of what I include here.

```
\frontmatter
\title{MyProject}
\author{Héctor Manuel Téllez Gómez}
\date{January 27, 2014 - \today}
\maketitle

\tableofcontents

\mainmatter
\input{NoteForTheReaders/NoteForTheReaders.tex}

\chapter{How to set up this template}
    \input{SettingUpTemplate/SettingUpTemplate.tex}

\chapter{First Chapter}
    \begin{center} February 17, 2014 \end{center}
    Chapter about the first chapter. 
    \section{Section 1}
    \input{Input1/input1.tex}
    
    \section{Section 2}    
    \input{Input2/input2.tex}
```

## Packages used:

The default list of packages used are:
- amsmath
- amsthm
- amssymb
- array
- color
- courier
- dsfont
- float
- embedfile
- enumitem
- geometry
- inputenc
- hyperref
- listings
- mathrsfs
- mathtools
- titlesec

You can optionaly add a file named config.tex (In your main directory) and add new packages or new preamble definitions there.

## Bibtex

You can optionaly add a file named bibtex.bib(In your main directory) and it will be taken as the bibliography references file.