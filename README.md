# Beyond Attribution: A Falsifiability Framework for Reliable Credit Risk Explanations

This repository contains two versions of the research paper on explainable AI for credit risk modeling.

## Repository Structure

### Original_Paper/
Contains the original paper in custom LaTeX format.

**Main Files:**
- `main.tex` - Main document file
- `main.pdf` - Compiled original paper (15 pages)
- `references.bib` - Bibliography in APA format
- `sections/` - Individual section files
  - `0_Abstract.tex`
  - `2_Introduction.tex`
  - `4_Literature_Review.tex`
  - `3.2_Methodology.tex`
  - `6_Results.tex`
  - `7_Conslusion.tex`
  - `8_Appendix.tex`
- `results/figures/` - All figures and plots
- `german_credit_record.csv` - Dataset used in the study

### IEEE_Access_Version/
Contains the paper converted to IEEE Access journal format.

**Main Files:**
- `credit_risk_ieee.tex` - Main IEEE Access formatted document
- `credit_risk_ieee.pdf` - Compiled IEEE Access paper (12 pages)
- `credit_risk_ieee.bbl` - Compiled bibliography (IEEE numerical format)
- `references.bib` - Bibliography file
- `ieeeaccess.cls` - IEEE Access document class
- `IEEEtran.bst` - IEEE bibliography style
- Font files (`t1-formata-*.pfb`, `t1-times-*.pfb`, etc.)

**Figures:**
- `architecture_diagram.png` - System architecture (Figure 1)
- `shap_german_credit_record_bagnn_100_bar.png` - SHAP bar plot
- `shap_german_credit_record_bagnn_100_dot.png` - SHAP summary plot
- `shap_german_credit_record_bagnn_100_waterfall_row0.png` - Local explanation waterfall
- `Relibility_Test.png` - Reliability diagnostics
- `feature_importance.png` - Feature importance visualization

## Key Differences Between Versions

| Aspect | Original | IEEE Access |
|--------|----------|-------------|
| Format | Single-column A4 | Two-column IEEE |
| Pages | 15 pages | 12 pages |
| Citations | APA style (`\parencite`) | IEEE numerical (`\cite`) |
| Sections | Unnumbered | Numbered |
| Figures | TikZ + PNG | PNG only (TikZ converted) |
| Bibliography | APA format | IEEE numerical format |

## Compilation Instructions

### Original Paper
```bash
cd Original_Paper
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### IEEE Access Version
```bash
cd IEEE_Access_Version
pdflatex credit_risk_ieee.tex
bibtex credit_risk_ieee
pdflatex credit_risk_ieee.tex
pdflatex credit_risk_ieee.tex
```

## Abstract

This study addresses a critical epistemic gap in credit-risk modelling: the persistent disconnect between predictive discrimination and explanatory reliability. While modern ensemble methods such as Bagged Neural Networks (BagNN) and Boosting establish strong predictive baselines in standard benchmarks, our results show that predictive success alone provides no assurance that a model's explanations are trustworthy or decision-relevant.

## Keywords

Explainable AI, Credit Risk, SHAP, Model Interpretability, Falsifiability, Financial Machine Learning

## Authors

Anonymous (under review)

## License

[To be added upon publication]

## Citation

[To be added upon publication]
