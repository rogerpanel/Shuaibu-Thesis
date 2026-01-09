# Dissertation LaTeX Project

## Title
**Assessing the Impacts of Urbanization on Plant Diversity and Ecosystem Functioning in Tropical Cities: A Case Study of Benue State, Nigeria**

## Author
Shaibu Ochoche

## Academic Information
- **Degree**: Doctor of Biological Sciences
- **Field**: 1.5.15 Ecology
- **Institution**: Российский Университет Дружбы Народов имени Патриса Лумумбы (RUDN University)
- **Institute**: Institute of Ecology
- **Scientific Advisor**: Dr. Pinaev Vladimir Evgenievich
- **Year**: 2025

## Project Structure

```
dissertation_final/
├── main.tex                    # Main LaTeX document
├── chapters/                   # Chapter files
│   ├── 00_frontmatter.tex     # Title page and table of contents
│   ├── 01_introduction.tex    # Introduction
│   ├── 02_literature_review.tex   # Chapter 1: Literature Review
│   ├── 03_methodology.tex     # Chapter 2: Research Methodology
│   ├── 04_results_discussion.tex  # Chapter 3: Results and Discussion
│   ├── 05_conclusion.tex      # Conclusion
│   ├── 06_recommendations.tex # Recommendations
│   ├── 07_references.tex      # References
│   └── 08_appendices.tex      # Appendices
├── figures/                    # All figures and images (74 files)
│   ├── figure_001.jpeg
│   ├── figure_002.jpeg
│   └── ... (and more)
└── README.md                   # This file
```

## Compilation Instructions

### Prerequisites
Ensure you have a LaTeX distribution installed:
- **Windows**: MiKTeX or TeX Live
- **Mac**: MacTeX
- **Linux**: TeX Live

```bash
# Ubuntu/Debian
sudo apt-get install texlive-full

# macOS (with Homebrew)
brew install --cask mactex

# Or use a lightweight installation
sudo apt-get install texlive-latex-base texlive-fonts-recommended texlive-latex-extra
```

### Compiling the Dissertation

#### Option 1: Using pdflatex (Recommended)

```bash
cd dissertation_final
pdflatex main.tex
pdflatex main.tex  # Run twice for proper references and table of contents
```

#### Option 2: Using latexmk (Automated)

```bash
cd dissertation_final
latexmk -pdf main.tex
```

#### Option 3: Full Compilation Sequence

For a complete compilation with all cross-references:

```bash
cd dissertation_final
pdflatex main.tex
pdflatex main.tex
pdflatex main.tex  # Third run ensures all references are resolved
```

### Expected Output
- **main.pdf**: Final compiled dissertation (approximately 150-200 pages)

## Compiling on Overleaf

1. Create a new project on [Overleaf](https://www.overleaf.com)
2. Upload all files maintaining the directory structure:
   - Upload `main.tex` to the root
   - Create `chapters/` folder and upload all chapter files
   - Create `figures/` folder and upload all figure files
3. Set the main document to `main.tex`
4. Click "Recompile"

**Note**: Due to the large number of figures (74 files), you may need an Overleaf premium account or split the upload into batches.

### Alternative: Upload as ZIP

1. From your local machine, create a ZIP file:
   ```bash
   cd dissertation_final
   zip -r dissertation.zip *
   ```
2. Upload the ZIP file to Overleaf via "New Project" → "Upload Project"

## Document Features

### Packages Used
- **Language Support**: Russian and English (babel, fontenc)
- **Graphics**: graphicx, caption, subcaption, float
- **Mathematics**: amsmath, amsfonts, amssymb
- **Tables**: booktabs, array, longtable, multirow
- **References**: natbib, hyperref
- **Layout**: geometry, setspace, fancyhdr

### Page Layout
- **Paper Size**: A4
- **Margins**: Left: 3cm, Right: 2cm, Top/Bottom: 2.5cm
- **Line Spacing**: 1.5 (onehalfspacing)
- **Font Size**: 12pt

### Figures
All figures are referenced using `\includegraphics` and are located in the `figures/` directory. To reference a figure in the text:

```latex
See Figure \ref{fig:figure_001_jpeg} for details.
```

## Content Overview

### Chapter 1: Literature Review
- Conceptual clarifications (urbanization, LULC, plant diversity, etc.)
- Review of related concepts and approaches
- Theoretical framework (Landscape Ecology, SAR Theory, IDH, Urban Scaling)
- Empirical review (global, African, and Nigerian studies)
- Research gaps and conceptual framework

### Chapter 2: Research Methodology
- Research design
- Study area (Makurdi and Otukpo, Benue State, Nigeria)
- Data requirements and sources
- LULC analysis using Random Forest classification
- Plant diversity assessment
- Ecosystem functioning and urbanization impact modeling
- Statistical analysis (ANOVA, regression)

### Chapter 3: Results and Discussion
- LULC classification results and dynamics (1990-2024)
- Plant composition and biodiversity patterns
- Soil properties across urban gradients
- Vegetation index analysis (NDVI/EVI)
- Relationship between urbanization metrics and ecosystem functioning
- Integrated assessment and ecological implications

### Back Matter
- **Conclusion**: Summary of key findings and limitations
- **Recommendations**: Policy recommendations for urban planning
- **References**: Complete bibliography
- **Appendices**: Additional data and documentation

## Key Findings

1. **Urban Expansion**: Built-up areas increased by 517% between 1990 and 2024
2. **Biodiversity Loss**: Clear declining trend in plant diversity from rural to urban areas
3. **Soil Degradation**: Significant increase in soil pH in urban areas
4. **Vegetation Decline**: NDVI/EVI showed substantial declines toward urban centers
5. **Population Pressure**: Population density was the strongest predictor of vegetation greenness decline

## Troubleshooting

### Common Issues

#### Error: "File not found"
- Ensure all chapter files are in the `chapters/` directory
- Check that figure files are in the `figures/` directory
- Verify file names match exactly (LaTeX is case-sensitive)

#### Error: "Undefined control sequence"
- Ensure all required packages are installed
- Run `pdflatex` multiple times to resolve cross-references

#### Error: "Too many open files" or slow compilation
- This can happen with many figures. Try compiling with `-shell-escape` or reduce image resolution

#### Figures not displaying
- Check that images exist in `figures/` directory
- Verify image file extensions (jpeg, png, pdf)
- Ensure `\graphicspath{{figures/}}` is set correctly

## Customization

### Changing Fonts
To use different fonts, modify the preamble in `main.tex`:

```latex
\usepackage{times}  % Times font
% or
\usepackage{palatino}  % Palatino font
```

### Adjusting Margins
Modify the geometry package settings in `main.tex`:

```latex
\geometry{
    a4paper,
    left=3cm,    % Adjust as needed
    right=2cm,   % Adjust as needed
    top=2.5cm,
    bottom=2.5cm
}
```

### Bibliography Style
The project uses natbib. To change citation style:

```latex
\bibliographystyle{plainnat}  % or abbrvnat, unsrtnat, etc.
```

## Version Information

- **Created**: January 2025
- **Original Format**: Microsoft Word (.docx)
- **Converted to**: LaTeX
- **Conversion Tools**: pandoc, python-docx, custom Python scripts
- **Figures Extracted**: 74 images (JPEG and PNG formats)

## License

This dissertation is the intellectual property of Shaibu Ochoche and RUDN University. All rights reserved.

## Contact

For questions regarding this dissertation:
- **Author**: Shaibu Ochoche
- **Advisor**: Dr. Pinaev Vladimir Evgenievich
- **Institution**: RUDN University, Institute of Ecology

## Acknowledgments

This LaTeX conversion was created to facilitate:
- Easy compilation and formatting
- Professional typesetting
- Cross-referencing and indexing
- Integration with academic publishing workflows

---

**Note**: This README provides comprehensive instructions for compiling and working with the dissertation LaTeX files. For technical support with LaTeX compilation, consult your institution's IT department or LaTeX community forums.
