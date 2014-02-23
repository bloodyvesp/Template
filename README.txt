LatexTemplate
=============

Default personal settings that I use while writing in latex.

_______________________________________________________________________
This project is to be included in a latex project. 
It has the most common libraries and definitions that 
I use and that not conlfict with many other things. 
(First compiling will return no errors, no bad boxes, no warnings, it is up to you
to keep it that way).



[[SETUP]]
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

