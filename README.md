Why this package
================
There is a lot of common mathematical notation, like constants or function
spaces, that should be typset consistently.
One _could_ introduce appropriate commands via TeX's \newcommand, e.g.
`\newcommand{\cfn}{\mathrm{C}}` and then use `\cnf([-1,1],\mathbb{R})`
for the space of continuous functions from the unit interval into the reals.
But this approach comes with some disadvantages, the main one being that even
if all additional annotations theoretically could be handled by optional
arguments (e.g. to typset the class `C^{(1)}` of continuously differentiable
functions, or the shorthand notation `C[-1,1] := C([-1,1],\mathbb{R})`), in
most cases it would not reflect the "typical" mathematical notation.

In my personal view, it would be desirable to mimic and reflect the usual
mathematical notation in custom commands, e.g., to be able to write
`\cfn(1)[-1,1]` for the class `\mathrm{C}^{(1)}[-1,1]`.
This is where the `xparse` LaTeX-package becomes very, _very_ handy.

For some further impressions, simply compile `sample.tex` and take a look at
its source.
The package `mathcommon.sty` itself is hopefully commented in sufficient 
detail to enable you (a) to use and (b) to extend it according to your needs.

Have fun typesetting. :)
