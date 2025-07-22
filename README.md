# Blei beamer theme

A clean and minimal Beamer theme mimicking David Blei's presentation from his [Variational Inference tutorial](https://youtu.be/DaqNNLidswA?si=HxNOvryN041XVdjg) and developed for academic presentations.

See [`example.pdf`](./example.pdf) for a complete example of the theme in action, showcasing all features and styling options. The source code for that is in [`example.tex`](./example.tex), but with images and other assets lacking to keep things simple.

- Clean, minimal design with serif fonts (Bitstream Charter)
- Simple navigation with page numbers in footer
- Customizable grey boxes for highlighting content
- Built-in bibliography support with `biblatex`
- Overlay functionality for emphasis
- Automatic section outline slides
- Optimized for clean academic presentations

## Installation

1. Download [`beamerthemeblei.sty`](./beamerthemeblei.sty) or clone the repo
2. Place it in your local texmf directory:
   ```
   ~/texmf/tex/latex/local/beamerthemeblei.sty
   ```

## Usage

### Basic usage

```latex
\documentclass[10pt,xcolor={dvipsnames}]{beamer}

\usetheme{blei} % <---- Use the theme

\title{Your Presentation Title}
\author{Your Name}
\date{\today}

\begin{document}

\maketitle

\begin{frame}{Your First Slide}
    Content goes here...
\end{frame}

\end{document}
```

### With bibliography

```latex
\documentclass[10pt,xcolor={dvipsnames}]{beamer}

\usetheme{blei}
\addbibresource{your-bibliography.bib}

% Your content...

% Add references at the end
\insertreferences

\end{document}
```

### Some features

All features are on display in [`example.pdf`](./example.pdf); its source code is in [`example.tex`](./example.tex).

#### Grey boxes
Highlight important content with grey boxes:
```latex
\greybox{Your highlighted content here}
```

#### Overlay text
Create overlay text for emphasis:
```latex
\overlay{Important message}
```

#### Wide item separation
Add extra spacing between list items:
```latex
\begin{itemize}
\widesep
\item First item
\item Second item
\end{itemize}
```

## Credits and license

Many thanks go to David Blei, not in the least for helping me understand VI!

Released under MIT license.