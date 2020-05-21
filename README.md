# MScAIThesisUL

This template was laregly built following the tutorial in overleaf - https://www.overleaf.com/learn/latex/How_to_Write_a_Thesis_in_LaTeX_(Part_1):_Basic_Structure

One noted challenge faced was in getting the bibliography to show, which was due to the need to included the configuration backend=bibtex when loading the biblatex package

\usepackage[style=authoryear,sorting=none,backend=bibtex]{biblatex}

I also manually added some of the items to the table of contents using the filecontents package 
e.g.
%to ensure you start on a new page
\clearpage
% add this to include the Bibliography in the ToC
\addcontentsline{toc}{chapter}{Bibliography}


I have set 5 variables for the title, name, id, supervisor name and date which are all displayed on the front page

\newcommand{\ThesisTitle}{My Thesis in the study of AI}
\newcommand{\AuthorName}{Student Name}
\newcommand{\AuthorID}{student ID}
\newcommand{\SupervisorName}{Add Supervisor Name}
\newcommand{\ThesisDate}{26 August 2020}
