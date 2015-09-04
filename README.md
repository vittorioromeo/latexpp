# latexpp
C++14 simple LaTeX preprocessor intended for personal use.

*...because I don't feel like learning LaTeX syntax.*

---

```
% Define macro with body
%!group(macro_name)(code_before_body)(code_after_body)

% Example: bash highlighting with minted
% Definition:
%!group(bash)(\begin{minted}[mathescape, linenos, numbersep=5pt, gobble=2, frame=lines, framesep=2mm, fontsize=\footnotesize]{bash})(\end{minted})

% Usage:
!!(bash)
!!{
    #!/bin/bash
    cd /home/hello/world
!!}
```

