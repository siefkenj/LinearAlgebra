# MultivariableCalculus
A textbook for multivariable calculus

## Compiling

This textbook is compiled with
    
    cd src/
    xelatex -shell-escape MultivariableCalculus.tex
    xelatex -shell-escape MultivariableCalculus.tex

Note that to get the index to appear, you must compile the document
twice.
Alternatively, if you have `arara` installed you can run

    cd src/
    arara MultivariableCalculus


_Multivarialbe Calculus_ relies hevily on the `tikz` and `pgfplots` 
package for LaTeX, so make sure you have it installed.
