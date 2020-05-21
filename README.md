# latexpp
C++14 simple LaTeX preprocessor intended for personal use.

---

```
% Define macro with body
%!group(macro_name)(code_before_body)(code_after_body)

% Example: bash highlighting with minted
% Definition:
%!group(bash)(\begin{minted}[mathescape, linenos]{bash})(\end{minted})

% Usage:
!!(bash)
!!{
    #!/bin/bash
    cd /home/hello/world
!!}
```

Result:

```
\begin{minted}[mathescape, linenos]{bash}
    #!/bin/bash

    latexpp ./thesis.lpp > ./thesis.tex
    pdflatex -shell-escape ./thesis.tex && chromium ./thesis.pdf
\end{minted}
```

---

Real-life example: [veeForum/latex](https://github.com/SuperV1234/veeForum/tree/master/latex)

