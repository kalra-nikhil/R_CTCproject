# CTCproject

*CTCproject* is an R and Quarto-based project analyzing Circulating Tumor Cells (CTCs) released during diagnostic breast biopsies.

# Project Overview
CTCproject is focused on statistical considerations for enumeration of Circulating Tumor Cells (CTCs) released during diagnostic biopsies in breast cancer patients.

CTCs represent tumor cells that have successfully detached from the primary lesion or metastatic site(s) and entered the bloodstream and currently a major focus of cancer research due to their vital role in metastatic process. It is estimated that a tumor releases thousands of tumor cells into circulation every day. Very few of them are actually able to survive and colonize distant organs to establish secondary tumors. Majority of them perish soon after they enter the bloostream due to different mechanisms, such as shear stress, anoikis (apoptosis due to dissociation from neighbouring cells and Extracellular matrix), attack from body's immune response, nutrient deprivation and metabolic changes.

Their detection and enumeration in blood is a technical challenge due to their rarity in blood (1 CTC every 10^6-10^8 normal cells) and heterogeneity (lack of universal CTC markers). Many enrichment techniques have been commercialised and in developmental phase for their isolation and enumeration.

In CTCproject, I used two different techniques to detect and count them in peripheral blood using liquid biopsy. I'm specifically looking for their increased release in blood due to tissue injury during breast biopsies. Since it is an early disease setting, baseline CTC counts are expected to be very low. Moreover detecting the increase of CTCs due to biopsies is challenging.

# Project Structure
- `index.qmd`: Project introduction and background
- `Rscripts/`: All analysis scripts in sequential steps
- `ctc_full_report.qmd`: Combined comprehensive report (rendered output of all scripts)

# How to Render the Full Report for complete analysis:
```bash
quarto render ctc_full_report.qmd
```
# How to preview the project locally with live updates:
```bash
quarto preview
```
# When to Use

- **quarto render:** When you want to **generate final HTML, PDF, DOCX** output.
- **quarto preview:** When you want to **view index.qmd live in the browser** and see automatic refreshes when you edit.

# Requirements
R version: 4.5.0
Quarto version: 1.7.32
R packages: render Rscripts/loading_packages.qmd

# Citation
If you use this work, please cite:
https://github.com/kalra-nikhil/CTCproject
Statistical considerations for enumeration of CTCs in breast cancer.
