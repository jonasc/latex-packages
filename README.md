# latex-packages
A documentation of good LaTeX packages an how to use them

# Mathematics

## [delimset](https://ctan.org/pkg/delimset) ([pdf](http://mirrors.ctan.org/macros/latex/contrib/delimset/delimset.pdf))

“*delimset* is a LaTeX2ε package to typeset and declare sets of delimiters in math mode
whose size can be adjusted conveniently.”

- It allows to use, e.g., `\brk*{…}` instead of `\left(…\right)` -- note the `*`
- It can also be used without automatic resizing, e.g., `\brk{…}` means `(…)` and `\brk[c]{…}` means `\{…\}`
- You can define your own commands, e.g., `\newcommand{\ceil}{\delim\lceil\rceil}` can then be used like `\brk`:
  - `\ceil{…}` uses the normal size
  - `\ceil*{…}` uses automatic size
  - `\ceil!{…}` uses `\big` as a size modifier (`2`, `3`, and `4` instead of `!` uses `\Big`, `\bigg`, and `\Bigg`)
- Can also be used, e.g., for sets `\set` and conditional sets `\setcond`
