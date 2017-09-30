# LinearAlgebra
A textbook for Linear Algebra

## Compiling

This textbook is compiled with
    
    cd src/
    xelatex -shell-escape LinearAlgebra.tex
    xelatex -shell-escape LinearAlgebra.tex

Note that to get the index to appear, you must compile the document
twice.
Alternatively, if you have `arara` installed you can run

    cd src/
    arara LinearAlgebra


_Linear Algebra_ relies heavily on the `tikz` and `pgfplots` 
package for LaTeX, so make sure you have it installed.

##Exercises

A `\begin{exercises}...\end{exercises}` environment is provided
for end-of-section exercises.  As well, a custom `\begin{problist}...\end{problist}`
environment is provided.  It should be used like an `enumerate` only with
`\prob` replacing `\item`.  `\prob` accepts an optional argument which becomes
a superscript on the problem number.

For example,

    \begin{problist}
        \prob Abc
        \prob[xx] Efg
        \prob[yy] Hjk
    \end{problist}

would be typeset as _1 Abc, 2^{xx} Efg, 3^{yy} Hjk_.  These problem annotations should
be used to describe the source of a problem.  For example `\prob[\openstax]` would
mark a problem as coming from the Openstax project.
