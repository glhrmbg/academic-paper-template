## Academic Paper Template - abnTeX2

An English template for academic papers using the abnTeX2 class, compliant with ABNT NBR 6022:2018 standards.

### Features

- **LaTeX Template**: Complete document structure for academic articles
- **English Language**: Template configured for English-language publications
- **ABNT Compliant**: Follows Brazilian ABNT standards for academic publications
- **Lorem Ipsum Content**: Placeholder text for easy customization
- **Comprehensive Structure**: Includes all standard sections of academic papers
- **Bibliography Support**: Pre-configured BibTeX integration
- **Professional Formatting**: Publication-ready layout and typography

### File Structure

```
├── paper.tex                    # Main document file
├── pretextual/
│   ├── preamble.tex             # Package imports and configurations
│   └── abstract.tex             # Abstract and keywords
├── chapters/
│   ├── introduction.tex         # Introduction section
│   ├── methodology.tex          # Materials and Methods
│   ├── results.tex              # Results and Discussion
│   ├── conclusion.tex           # Conclusion
│   └── acknowledgements.tex     # Acknowledgements
├── tables/                      # Table files (if needed)
│   └── result-table-1.tex       # Table 1
├── images/                      # Figure files
│   └── result-figure-1.jpg      # Figure 1
├── .tex/                        # abnTeX2 class files
│   ├── abntex2.cls
│   ├── abntex2cite.sty
│   ├── abntex2abrev.sty
│   └── [other abnTeX2 files]
├── reference.bib                # Bibliography database
└── README.md                    # This file
```

### Quick Start

1. **Clone or Download** this template to your local machine
2. **Customize** the document information in `pretextual/preamble.tex`:
   - Title, authors, affiliations
   - PDF metadata
   - Contact information
3. **Replace** lorem ipsum content with your research:
   - Update `pretextual/abstract.tex` with your abstract
   - Modify chapter files with your content
   - Add your references to `reference.bib`
4. **Compile** using LaTeX:
   ```bash
   pdflatex paper.tex
   bibtex paper
   pdflatex paper.tex
   pdflatex paper.tex
   ```

### Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- abnTeX2 package (included in .tex/ folder)
- BibTeX for bibliography processing

#### Required LaTeX Packages

The template uses several LaTeX packages that should be included in most modern LaTeX distributions:

- `ebgaramond` - Font package
- `graphicx` - Graphics support
- `amsmath`, `amsfonts`, `amssymb` - Mathematics support
- `siunitx` - SI units formatting
- `booktabs` - Professional tables
- `hyperref` - PDF hyperlinks
- `pgfplots` - Plot generation
- And others (see `pretextual/preamble.tex`)

### Customization

#### Document Information
Edit the following in `pretextual/preamble.tex`:
```latex
\titulo{Your Paper Title}
\autor{Author Names and Affiliations}
\local{Your Country}
```

#### Content Structure
The template follows the standard academic paper structure:

1. **Abstract** - Brief summary with keywords
2. **Introduction** - Background and motivation
3. **Materials and Methods** - Methodology description
4. **Results and Discussion** - Findings and analysis
5. **Conclusion** - Summary and future work
6. **Acknowledgements** - Credits and funding information
7. **References** - Bibliography

#### Adding Figures and Tables
- Place figures in the `images/` directory
- Create table files in the `tables/` directory
- Reference them using `\ref{label}` commands

#### Bibliography
Add your references to `reference.bib` following BibTeX format:
```bibtex
@article{key,
  title={Paper Title},
  author={Author Name},
  journal={Journal Name},
  year={2023}
}
```

### License

This template is based on the abnTeX2 class, which follows the LaTeX Project Public License (LPPL). You are free to use, modify, and distribute this template for academic purposes.

### Support

For questions about:
- **abnTeX2 class**: Visit [abnTeX2 official website](https://www.abntex.net.br/)
- **LaTeX general help**: Consult [LaTeX documentation](https://www.latex-project.org/help/documentation/)
- **This template**: Open an issue in the repository
