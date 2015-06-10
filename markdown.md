---
title: Markdown \#Citymash handout
---

### What this session will cover 
* The problems with proprietary file formats
* 

### Problems with proprietary file formats

* Proprietary file formats encode text in binary format. 
* There are different ways of accessing propitiatory formats: 
    - [A Wordstar emulator](https://goo.gl/Nuystv). 
    - We can use OpenOffice or Libre Office to open most Doc and Docx files, but we cannot always [^1] use word to open OpenOffice (odt) files. 

## Text files 

> 'Refers to textual data in ASCII format. Plain text is the most portable format because it is supported by nearly every application on every machine. It is quite limited, however, because it cannot contain any formatting commands.' https://archive.org/details/wordstar_2.26_osborne1_1981_micropro

Because text files use minimal encoding understood by most computers they are very stable file formats that can easily move across different devices without compatibility issues. 

To demonstrate this we can try opening [old plain text files](http://textfiles.com/100/whytext.oct). This site collects text files primarily from the years 1980-95 all of which can still be opened both in your browser and with software on your computer. If we compare this to files produced by word processors we can have compatibility and formating issues from files produced by an earlier version of the same software. Working with an individual file this may not be such a problem but if we are working with a whole collection of different documents we can see potential difficulties emerging. 

### Some potential problems with plain text

Whilst plain text files are great in many ways, one of the potential problems with them is that they are a bit plain. Often we need to structure documents in some ways. Some text serves as headings, other points we might want to emphasise, we may want to separate quoted text from the rest of the text. This isn't about formating the text yet but purely about the logical structure of the text. We can 'mark' these aspects of text in different ways. One solution would be to use HTML, however a problem with using HTML is that it is already more concerned with formating how text will be displayed. Another potential option is to use LaTeX, which is a method designed for producing well typeset documents, however the syntax (language) has a bit of a learning curve and LaTeX documents are not primarily designed for the web. 

#### LaTeX example

    \documentclass[12pt]{article}

    \setlength{\parskip}{1.2ex}    % space between paragraphs
    \setlength{\parindent}{2em}    % amount of indention
    \setlength{\textwidth}{175cm}      % default = 6.5"
    \setlength{\oddsidemargin}{-5mm}   % default = 0"
    \setlength{\textheight}{225mm}     % default = 9"
    \setlength{\topmargin}{-12mm}      % default = 0"

        %  ---  define your own commands!! ---
    \newcommand{\iii}{\indent \indent \indent}  % triple-depth indent

    \title{A Sample \LaTeX\  Document}
    \author{Schl\oe ff\d{o}nffl\t{oo}\ae g\"{e}n, \L\"{a}rs}
    \date{July 14, 1992}

    \begin{document}
                   
    \maketitle

    \subsection{Spacing in the source text}
    The ends  of words and sentences are marked
      by   spaces. It  doesn't matter how many
    spaces
    you
    type; one is as good as                        100.
    The       end of   a line counts as a space.

    One   or more   blank lines denote the  end of  a paragraph.

    Since any number of consecutive spaces are treated like a single one, the
    formatting of the input file makes no difference to \TeX, but it makes a
    difference to you.  When you use \LaTeX, making your input file as easy to
    read as possible will be a great help as you write your document and when
    you change it.  Keep typed lines {\bf short} in length, and use
    \verb9 % comments9.                             % like this!

    Because printing is different from typewriting, there are a number of things
    that you have to do differently when preparing an input file than if you were
    just typing the document directly.  Quotation marks like ``this'' have to
    be handled specially.
     
    \end{document}      
[^2]

Although LaTeX is perfect for typesetting documents that will be printed, something we will return to later, it can be to cumbersome for short documents which may not necessarily be intended primarily for printing. 

## What is Markdown?

Whilst plain text files are great in many ways, one of the potential problems with them is that they are a bit plain. Often we need to structure documents in some ways. Some text serves as headings, other points we might want to emphasise, we may want to separate quoted text from the rest of the text. This isn't about formating the text yet but purely about the logical structure of the text. We can 'mark' these aspects of text in different ways. One solution would be to use HTML, however a problem with using HTML is that it is already more concerned with formating how text will be displayed.



Plain text that is not computationally tagged, specially formatted, or written in code.
* markdown is a syntax for setting out the structure of the document in a way which is human readable. 
* there are a number of different 'flavours' of markdown but they all have similar conventions 
* the idea of markdown is to provide minimal amounts of 'markup' to allow the focus on writing. 
* it is easy to convert between markdown and html but also other formats using pandoc 


## How to write in Markdown

* no special software needed. any text editor (not word processor can be used)
* online 

### Some things to try with Mardown 
These are a few different places we can play around with converting our markdown file into other formats. 

#### Markdown to HTML

## Pandoc 

Pandoc is a software 

allows you to include references in a plain text format using bibtex files 
.bib files are bibliographic files in plain text. 
they have been around since the 80s. 


## Resources

* markdown cheat sheet 
* pandoc 
* http://whatismarkdown.com/

---
[^1]: It is not always clear whether it is possible or not. It can depend on the version of the Word Processor being used at each end, the operating system and the type of files embedded in the document. 

[^2]: http://spot.colorado.edu/~sitelic/samplecode/latex/sample.html 