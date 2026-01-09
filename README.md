# Dissertation: Assessing the Impacts of Urbanization on Plant Diversity and Ecosystem Functioning

## Project Overview

This repository contains the doctoral dissertation of **Shaibu Ochoche** on the impacts of urbanization on plant diversity and ecosystem functioning in tropical cities, with a focus on Benue State, Nigeria.

## Author Information

- **Name**: Shaibu Ochoche
- **Degree**: Doctor of Biological Sciences
- **Field**: 1.5.15 Ecology
- **Institution**: RUDN University (Российский Университет Дружбы Народов имени Патриса Лумумбы)
- **Institute**: Institute of Ecology
- **Scientific Advisor**: Dr. Pinaev Vladimir Evgenievich
- **Year**: 2025

## Repository Contents

### Main Files

1. **BshaibuIO THESIS UPDATED.docx** - Original dissertation in Microsoft Word format
2. **dissertation_final/** - LaTeX version of the dissertation ready for compilation
   - Full LaTeX source code
   - All chapter files organized
   - 74 extracted figures
   - Compilation instructions in README

### Dissertation Structure

The dissertation examines:
- **Land Use/Land Cover (LULC) Change**: Analysis of urban expansion from 1990-2024
- **Plant Biodiversity**: Assessment across rural, peri-urban, and urban gradients
- **Ecosystem Functioning**: Vegetation indices (NDVI/EVI) and soil indicators
- **Statistical Modeling**: Relationship between urbanization metrics and ecological impacts

## Quick Start

### Using the LaTeX Version

```bash
cd dissertation_final
pdflatex main.tex
pdflatex main.tex  # Run twice for proper cross-references
```

For detailed compilation instructions, see [dissertation_final/README.md](dissertation_final/README.md)

### Using Overleaf

1. Download the `dissertation_final` folder
2. Upload to [Overleaf](https://www.overleaf.com) as a new project
3. Compile to generate PDF

## Key Findings

1. **Urban Expansion**: Built-up areas increased by **517%** between 1990 and 2024
2. **Biodiversity Decline**: Plant diversity decreases significantly from rural to urban areas
3. **Vegetation Loss**: NDVI/EVI indices show substantial declines in urban centers
4. **Soil Alteration**: Urban areas exhibit significantly altered soil pH and nutrient properties
5. **Population Impact**: Population density is the strongest predictor of vegetation decline

## Research Methodology

- **Remote Sensing**: Landsat imagery (1990, 2010, 2024) with Random Forest classification
- **Field Surveys**: 33 vegetation plots across Makurdi and Otukpo LGAs
- **Soil Analysis**: Comprehensive soil sampling across urbanization gradients
- **Statistical Analysis**: ANOVA, regression modeling, and spatial analysis

## Figures and Data

- **Total Figures**: 74 images including:
  - LULC classification maps
  - Vegetation diversity charts
  - Soil property graphs
  - Statistical analysis results
  - Regression model outputs

All figures are available in the `figures/` directory and properly referenced in the LaTeX document.

## Document Formats

### Original Format
- **File**: BshaibuIO THESIS UPDATED.docx
- **Size**: ~5.2 MB
- **Format**: Microsoft Word

### LaTeX Format
- **Directory**: dissertation_final/
- **Main File**: main.tex
- **Chapters**: 8 chapter files + front/back matter
- **Compilation**: Standard LaTeX workflow

## Technical Details

### LaTeX Packages Used
- babel (Russian/English support)
- graphicx (figures)
- natbib (references)
- amsmath (equations)
- hyperref (cross-references)
- And more (see main.tex for full list)

### System Requirements
- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- pdflatex or similar LaTeX compiler
- Approximately 50MB free space for compilation

## Contributing

This is a completed academic dissertation. However, if you notice any issues with the LaTeX compilation or formatting, please open an issue.

## Citation

If you use this work or methodology in your research, please cite:

```
Shaibu, O. (2025). Assessing the Impacts of Urbanization on Plant Diversity and
Ecosystem Functioning in Tropical Cities: A Case Study of Benue State, Nigeria.
Doctoral Dissertation, RUDN University, Institute of Ecology.
```

## License

See LICENSE file for details.

## Acknowledgments

This research was conducted at the Institute of Ecology, RUDN University, under the supervision of Dr. Pinaev Vladimir Evgenievich.

## Contact

For questions about this research:
- **Author**: Shaibu Ochoche
- **Institution**: RUDN University, Institute of Ecology
- **Location**: Moscow, Russia

---

**Last Updated**: January 2025

**Note**: This repository contains both the original Word document and a professionally formatted LaTeX version suitable for academic publication and compilation on Overleaf.
