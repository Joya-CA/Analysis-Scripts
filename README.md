# Analysis-Scripts
All code to reproduce the analysis.

RQ1: Does the abundance of an AMF isolate introduced into a community change with isolate identity or host identity? 

## Data Descriptions (`/AMFAbundance/`)

| File Name                          | Description |
|-----------------------------------|-------------|
| `197198_syntheticDNA`             | QuantaSoft output of DAOM 197198 abundance using serial dilutions of synthetic DNA |
| `240448_syntheticDNA`             | QuantaSoft output of DAOM 240448 abundance using serial dilutions of synthetic DNA |
| `240720_syntheticDNA`             | QuantaSoft output of DAOM 240720 abundance using serial dilutions of synthetic DNA |
| `Inoculum_potential_2024_05_cleaned` | Cleaned data used to estimate inoculum potential |
| `RQ1_results_cleaned_ddPCR`       | Data used for AMF abundance statistical analysis |
| `SingleSpore_AllIsolates`         | QuantaSoft output of single spore extractions |
| `Cairance_DilutionFactors_All`   | Dilution factors used to convert copies/µL to copies/g root |
| `Variance_Longform_M24_M25`       | Cleaned results from variance extraction of individual hosts |

---

## How to Use

Open the appropriate R Markdown file and use the corresponding dataset(s) to reproduce the analysis. Run the code top-to-bottom.

| R Markdown File                                 | Corresponding Data Files |
|-------------------------------------------------|---------------------------|
| `RQ1_ddPCR_July_2025_Markdown.Rmd`             | `RQ1_results_cleaned_ddPCR`, `Variance_DilutionFactors_All` |
| `ProbeEfficiency_SporeNuclearAbundance_Markdown.Rmd` | `197198_syntheticDNA`, `240448_syntheticDNA`, `240720_syntheticDNA`, `SingleSpore_AllIsolates` |
| `Variance_ddPCR_Visualisations_July_2025.Rmd`  | `Variance_Longform_M24_M25`, `Variance_DilutionFactors_All` |

---

## Dependencies

- **R version**: 4.3.2  
---

## Data Reference (Key Variables)

| Variable        | Description                                                 |
|----------------|-------------------------------------------------------------|
| `copies_g`      | AMF abundance, calculated as copies per gram of root        |
| `treatment`     | AMF isolate identity (levels: Control, DAOM 197198, DAOM 240448, DAOM 240720) |
| `species`       | Host plant species (Gaillardia aristata, Festuca idahoensis, Bromus tecotrum, Taraxacum officinale) |
| `mesocosm_id`   | Unique ID for each mesocosm (experimental unit)             |
| `sample_id`     | Unique ID for each individual host within a mesocosm        |

---

##  Author

Joyalea Carson-Austin
Supervisor: Dr. Miranda Hart
University of British Columbia – Okanagan  
Master’s Thesis Research (2025)

---
This project is shared under the **CC BY-NC 4.0** license. Contact the author for reuse permissions.

