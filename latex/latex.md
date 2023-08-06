
<!-- # WYSIWYM - What You See Is What You Mean -->

## Table of contents
- [What is LATEX?](#what-is-latex)
- [Why learn LATEX?](#why-learn-latex)
- [Usage](#usage)
    - [Default](#default)
    - [Class types](#class-types)
    - [Page size and margins](#page-size-and-margins)
    - [External package](#external-package)
    - [Title, author and date information](#title-author-and-date-information)
    - [Bold, italics and underlining](#bold-italics-and-underlining)
    - [Adding images](#adding-images)
    - [Captions, labels and references](#captions-labels-and-references)
    - [Lists](#lists)
    - [Math](#math)
    - [Creating tables](#creating-tables)
- [Basic document structure](#basic-document-structure)
    - [Abstracts](#abstracts)
    - [Paragraphs and new lines](#paragraphs-and-new-lines)
    - [Chapters and sections](#chapters-and-sections)


### Reference: 
1. Overleaf ["Learn LaTeX in 30 minutes"](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)
2. Medium ["Writing LaTeX Documents In Visual Studio Code With LaTeX Workshop"](https://medium.com/@rcpassos/writing-latex-documents-in-visual-studio-code-with-latex-workshop-d9af6a6b2815)

Short | Detail
--|--
CTAN | [Comprehensive TeX Archive Network](https://www.ctan.org/)

# What is LATEX? 
***LaTeX*** is a tool for typesetting professional-looking documents. Your document is a plain text file interspersed with LaTeX commands used to express the desired (typeset) results. ***TeX engine*** which uses the commands embedded in your text file to guide and control the typesetting process, converting the LaTeX commands and document text into a professionally typeset PDF file. [1]

# Why learn LATEX?
It is a personal choice based on preferences, affinities, and documentation requirements.
  - support for typesetting extremely complex mathematics, tables and technical content for the physical sciences;
  - facilities for footnotes, cross-referencing and management of bibliographies;
  - ease of producing complicated, or tedious, document elements such as indexes, glossaries, table of contents, lists of figures;
  - being highly customizable for bespoke document production due to its intrinsic programmability and extensibility through thousands of free add-on packages. 


There are the three most important:  
- Focus on Content first, and let LaTeX deal all the formatting
- Easy Citations
- High-quality typography

# Usage
### Default
default font size is 10pt

### Class types

    \documentclass{article} % scientific paper
    \documentclass{resume} % CV/resume
    \documentclass{book}
    \documentclass{report}

### [Page size and margins](https://www.overleaf.com/learn/latex/Page_size_and_margins)
    \documentclass[12pt, letterpaper]{article}
    \documentclass[12pt, a4paper ]{article}
    \documentclass[12pt, legalpaper]{article}
### External package
    \usepackage{graphicx} %import graphics

### Title, author and date information
    \title{My first LaTeX document} % the document title
    \author{An Phung Van\thanks{Dung Nghiem Nguyen Viet}}
    \date{July 2023}

    \maketitle % use within the body of the document to typeset the title, author and date

### Bold, italics and underlining

    \textbf{...} % bold
    \textit{...} % italics
    \underline{...} % underline
    \emph{argument} % effect is reversed depends on the context

### Adding images

    \usepackage{graphicx} %LaTeX package to import graphics
    \graphicspath{{images/}} %configuring the graphicx package

    \includegraphics{...}  

### Captions, labels and references

[Captions, labels and references for image](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Captions,_labels_and_references)

[Captions, labels and references for table](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Captions,_labels_and_references_2)

### Lists
Unordered lists

    \begin{itemize}
        \item The individual entries are indicated with a black dot, a so-called bullet.
        \item The text in the entries may be of any length.
    \end{itemize}

Ordered lists

    \begin{enumerate}
        \item This is the first entry in our list.
        \item The list numbers increase with each entry we add.
    \end{enumerate}

### [Math](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#More_complete_examples)
    \usepackage{amsmath}% For the equation* environment

Inline 

    \( ... \)
    $ ... $
    \begin{displaymath} ... \end{displaymath}
### Creating tables

    \begin{center}
    \begin{tabular}{c c c}
    cell1 & cell2 & cell3 \\ 
    cell4 & cell5 & cell6 \\  
    cell7 & cell8 & cell9    
    \end{tabular}
    \end{center}
Adding borders

    \hline % horizontal 
    | % vertical, use between columns 

[Adding a Table of Contents](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_a_Table_of_Contents)

# Basic document structure
### Abstracts

    \begin{abstract}
        This is a simple paragraph at the beginning of the 
        document. A brief introduction about the main subject.
    \end{abstract}

### Paragraphs and new lines

    \usepackage{parskip}

    press ``enter'' twice
    \\
    \newline

### Chapters and sections

