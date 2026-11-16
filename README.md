# Nigeria–UK Cancer Diagnostic Pathways: Reproducible Scoping Review Analysis

## Overview

This repository documents a Python-based analysis of published evidence on cancer diagnostic pathways, referral practices, and barriers to timely diagnosis in Nigeria and the United Kingdom (UK). The analysis formed part of a comparative scoping review intended to map reported diagnostic pathways and identify practices that may be relevant to improving early cancer diagnosis in Nigeria.

The notebook documents the data-verification process, descriptive evidence mapping, diagnostic-pathway reporting assessment, thematic coding, regional summaries, and Nigeria–UK comparisons. It also includes a **preliminary screening** of intervention-effectiveness evidence.

**Project status:** Research analysis and manuscript preparation. This repository is a record of analytical work; the notebook is not itself a peer-reviewed publication.

## Research questions

1. What diagnostic pathways from symptom recognition to diagnosis were reported across Nigerian regions?
2. Which patient-, provider-, and health-system factors were associated with delays and late cancer diagnosis?
3. How did diagnostic and referral pathways reported in Nigeria compare with those reported in the UK?
4. Which referral practices and interventions identified in the evidence might be relevant to improving timely diagnosis in Nigeria?

## Evidence base

| Measure | Records |
|---|---:|
| Included publications | 242 |
| Nigerian publications | 42 |
| UK publications | 200 |
| Extracted factor findings (Sheet 3) | 979 |
| Extracted problem/intervention entries (Sheet 4) | 472 |
| Researcher-approved thematic decisions | 68 |
| Intervention entries flagged for further evidence interpretation | 91 |

**Counting note:** The factor and intervention figures are *extraction rows*, not additional independent publications, patients, or independently evaluated interventions. The 91 entries represent a review subset, not a finding that 91 interventions were effective.

## Notebook

The notebook contains the following stages:

- Verification of required input files and recording of SHA-256 file hashes.
- Validation of study identifiers and dataset linkage.
- Study-level descriptive summaries by country and research characteristics.
- Assessment of the specificity of diagnostic-pathway reporting.
- Nigerian regional evidence mapping.
- Automated framework mapping followed by researcher-approved thematic coding.
- Cross-checks of coding decisions, including 61 assigned themes and seven retained as unclassified.
- Nigerian factor summaries and Nigeria–UK diagnostic-pathway comparisons.
- A preliminary intervention-evidence screen and a 91-entry export for further interpretation.

**Interpretive limitations:** Reporting frequencies describe what included publications explicitly documented, not the prevalence of clinical events in patients. Differences between Nigerian and UK publications are descriptive and may reflect different cancer types, study designs, healthcare settings, and reporting practices. Recommendations and indirectly observed associations were not interpreted as proven intervention effectiveness.

## Input data

The notebook expects these five files, with their exact filenames:

```text
Sheet_1_clean(2).xlsx
Sheet_2_clean(3).xlsx
Sheet_3_clean(2).xlsx
Sheet_4_clean(2).xlsx
Nigeria_UK_Thematic_Coding_Framework.xlsx
```

The first four files contain cleaned, linked study extraction data. The fifth contains the thematic coding framework, not additional included studies.

**Data availability:** The required workbooks are not included in this repository package. Reproducing the computations requires access to these exact files or appropriately documented equivalent files. Full-text articles and any data for which redistribution is not permitted should not be uploaded without permission.

## Reproducibility

The notebook was developed for Google Colab and uses Python, `pandas`, and Excel-reading/writing support such as `openpyxl`.

1. Open the notebook in Google Colab.
2. Make the five required input workbooks available to the Colab session under their exact filenames.
3. Execute the notebook in sequence.
4. Inspect the file manifest, study-ID assertions, coded tables, and summary outputs.

Most sections use in-memory data frames and leave the original extraction workbooks unchanged. One cell produces an Excel analysis workbook:

```text
Nigeria_UK_RQ1_Pathways_Approved_Thematic_Coding.xlsx
```

A later cell creates a 91-entry intervention-evidence review CSV:

```text
RQ4_91_Evidence_Review.csv
```

Both outputs depend on the source files and code being executed successfully. Saved notebook outputs are retained from the supplied notebook; they should not be mistaken for a fresh execution of this repository version.

## Research integrity and attribution

The analytical record preserves source descriptions alongside standardized variables and retains review decisions, original coding flags, and researcher-approved coding outcomes. Ambiguous or insufficiently reported information was not automatically converted into confirmed clinical evidence. No claim of causal effect or intervention efficacy was inferred solely from the presence of an intervention recommendation.

**Researcher:** Ugochinyere Chiamaka Obinwanne

**Research context:** Comparative scoping review of cancer diagnostic pathways in Nigeria and the UK.

## Citation

If this repository is used or discussed, cite the author, repository title, version/date, and GitHub URL once published. A formal manuscript citation can be added after publication.
