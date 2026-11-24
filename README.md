# Indian Dietary Environmental Footprint Calculator

[![License: MIT](https://img.shields.io/badge/License-MIT-1b4332.svg)](LICENSE)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

A client-side web application and companion Excel workbook for quantifying **greenhouse gas (GHG) emissions**, **green water footprint**, **blue water footprint**, and **land use footprint** from Indian dietary intake (entered in grams).

## Key Features

- **Automatic Food Classification:** Maps typed food names (e.g., `Apple`, `Turmeric`, `Basmati Rice`, `Paneer`, `Toor Dal`) into 18 standardized Indian dietary categories using exact and token-level matching.
- **Raw & Cooked Weight Support:** Accepts intake in grams (`g`) for either raw ingredients or cooked/ready-to-eat dishes, converting cooked weights back to raw equivalents via standard cooking yield factors.
- **ICMR-NIN Benchmark Comparison:** Compares cumulative daily intake against the **ICMR-NIN 'My Plate for the Day' (Vegetarian)** reference (`2.30 kg CO₂-eq/day`, `2.35 m³/day` green water, `0.44 m³/day` blue water, `4.96 m²/day` land use).
- **Zero-Backend Deployment & CSV Export:** Runs entirely in the browser via GitHub Pages with local persistence and one-click CSV export.

## Repository Contents

| File | Description |
| :--- | :--- |
| `index.html` | Standalone browser application (HTML/CSS/JS) with auto-classification, cooking yield toggle, and citation tools. |
| `Indian_Diet_Environmental_Footprint_Calculator.xlsx` | Formula-driven Excel workbook (`INDEX`/`MATCH`, `SUMIFS`, `SUMPRODUCT`) with 18-category coefficients and lookup dictionary. |
| `CITATION.cff` | Machine-readable citation metadata for GitHub and Zenodo DOI archiving. |
| `LICENSE` | MIT License governing the software source code and interface. |

## Scientific Methodology & Data Sources

Per-kilogram environmental intensity coefficients across the 18 food groups (`Dairy`, `Dairy_Fat`, `Eggs`, `Fish`, `Fruits`, `Millets`, `Nuts_Oilseeds`, `Oils_Plant`, `Other_Cereals`, `Poultry`, `Processed_Other`, `Pulses`, `Red_Meat`, `Rice`, `Spices_Condiments`, `Sugars`, `Vegetables`, `Wheat`) and reference benchmarks are derived from:

1. **Joshi, N., & Raghuvanshi, R. S. (2025).** Exploring environmental footprints and socio-demographic characteristics of Indian diets. *Science of the Total Environment*, 967, 178781. https://doi.org/10.1016/j.scitotenv.2025.178781
2. **Green, R. F., Joy, E. J. M., Harris, F., Agrawal, S., Aleksandrowicz, L., Hillier, J., Macdiarmid, J. I., Milner, J., Vetter, S. H., Smith, P., Haines, A., & Dangour, A. D. (2018).** Greenhouse gas emissions and water footprints of typical dietary patterns in India. *Science of the Total Environment*, 643, 1411–1418. https://doi.org/10.1016/j.scitotenv.2018.06.258
3. **Mekonnen, M. M., & Hoekstra, A. Y. (2010, 2012).** Water Footprint Network crop and farm animal product datasets.
4. **Bognár, A. (2002) & EuroFIR (2008).** Weight yield conversion factors for cooked foods.

## How to Cite This Software

If you use this application in academic research, policy analysis, or teaching, please cite both the software authors and the underlying empirical studies:

> Alphonso, R., & Cheela, V. R. S. (2026). *Indian Dietary Environmental Footprint Calculator* (Version 1.0.0) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX

```bibtex
@software{alphonso_cheela_2026_diet_footprint,
  author       = {Alphonso, Rachael and Cheela, Venkata Ravi Sankar},
  title        = {Indian Dietary Environmental Footprint Calculator},
  year         = {2026},
  version      = {1.0.0},
  publisher    = {Zenodo},
  license      = {MIT},
  doi          = {10.5281/zenodo.XXXXXXX},
  url          = {https://doi.org/10.5281/zenodo.XXXXXXX}
}
```

## License & Attribution Scope

- **Software Code:** Copyright &copy; 2026 **Rachael Alphonso** and **Cheela Venkata Ravi Sankar**. Released under the [MIT License](LICENSE).
- **Underlying Datasets:** Empirical footprint values and dietary reference benchmarks remain subject to their original scholarly attributions (Joshi & Raghuvanshi, 2025; Green et al., 2018, CC BY 4.0).
