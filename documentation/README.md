### TODO ###

Design Section. Diagram with justification.

Planning section. Testing of each requirement.

Testing.

### Report Skeleton ###

Basically to make this as modular as possible and reduce the number of
conflicts I have a single root file which includes many other files.

In the root of the documentation directory I have two .tex file:
report.tex and abstract.tex

report.tex is the root tex file which includes all other tex files. 
In addition to including other tex files, report.tex also contains the
title page.

abstract.tex was included in the root directory because it will be a 
single file and it doesn't make sense to put it in its own directory.

I have broken down each section into its own folder in the following 
way:

Each directory has a root file with the same name as the directory. This
file contains the \section label followed by a paragraph or so long 
description of what this section is about. The other files in this 
directory are subsections that are included by the root file, they begin
with \subsection followed by all the relevant information in the 
subsection.

Try to follow this format as best as possible. Thanks.

### Bibliography ###
I will update information about editing the bib/bib.bib file soon.


### Adding Figures and Tables ###

I will add information about this soon

### Compilation ###
Here are the following steps to compile the document from the root 
directory in a linux command line:

```
pdflatex report 
biber report
pdflatex report
pdflatex report
```
