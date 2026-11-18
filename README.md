# Ki67-Breast-Cancer-Bioinformatics
Bioinformatics analysis of Ki-67 (MKI67) gene expression in breast cancer using the UALCAN database.
# MKI67 Expression Analysis in Breast Cancer

## Project Overview

This project investigates the expression of **MKI67**, a gene associated with cellular proliferation, in breast cancer.

The main objective was to determine whether MKI67 expression differs between normal breast tissue and breast tumour samples, whether its expression is associated with overall survival, and which other genes and biological pathways show related expression patterns.

This project uses publicly available gene-expression datasets and web-based bioinformatics tools.

## Research Questions

1. Is MKI67 expression higher in breast tumour samples compared with normal breast tissue?
2. Is MKI67 expression associated with overall survival in breast cancer patients?
3. Which genes show strong expression correlations with MKI67?
4. Which biological pathways are enriched among the selected correlated genes?

## Tools and Resources

- **PubMed:** Scientific literature review
- **UALCAN:** TCGA breast invasive carcinoma (BRCA) gene-expression and survival analysis
- **GEO2R:** Independent gene-expression analysis of GEO dataset GSE42568
- **Enrichr:** Biological pathway enrichment analysis
- **Microsoft Excel:** Organisation and interpretation of results

## Datasets

### TCGA-BRCA

- Normal breast tissue samples: 114
- Primary tumour samples: 1,097
- Gene analysed: MKI67
- Expression metric: Transcript per million (TPM)

### GEO: GSE42568

- Total samples: 121
- Normal breast samples: 17
- Breast cancer samples: 104
- Platform: GPL570 (Affymetrix Human Genome U133 Plus 2.0)

## Key Findings

### 1. MKI67 Expression

MKI67 expression was significantly higher in primary breast tumour samples compared with normal breast tissue in TCGA-BRCA.

- p-value: 1.624 × 10⁻¹²

### 2. Overall Survival

The overall survival analysis did not identify a statistically significant difference between the high and low/medium MKI67 expression groups.

- High-expression group: 267 patients
- Low/medium-expression group: 814 patients
- Log-rank p-value: 0.16

### 3. Gene Correlation Analysis

Several genes showed strong positive expression correlations with MKI67:

| Gene | Correlation coefficient |
|---|---:|
| KIF11 | 0.82 |
| KIF4A | 0.81 |
| CKAP2L | 0.81 |
| ASPM | 0.79 |
| CLSPN | 0.77 |

These genes are associated with processes such as mitosis, chromosome organisation and DNA replication.

### 4. Expression Analysis of Correlated Genes

KIF11, KIF4A and ASPM were also found to have significantly higher expression in primary tumour samples than normal breast tissue in TCGA-BRCA.

### 5. Pathway Enrichment

Enrichment analysis using the MSigDB Hallmark 2020 library identified:

- G2-M Checkpoint
- Adjusted p-value: 0.009606

The Reactome and KEGG results did not show statistically significant adjusted p-values among the reported top terms.

## Conclusion

The analysis indicates that MKI67 expression is significantly elevated in breast tumour samples and is strongly correlated with several genes involved in cell proliferation and cell-cycle regulation.

However, the overall survival analysis did not show a statistically significant association between MKI67 expression groups and overall survival.

These findings support an association between MKI67 expression and proliferative activity in breast cancer but do not establish a causal relationship.

## Limitations

- The analyses are observational and based on publicly available datasets.
- Correlation does not establish direct gene interaction or causation.
- Survival analysis may be influenced by clinical factors such as age, tumour stage, subtype and treatment.
- GEO2R contrast direction requires further verification before interpreting the direction of its MKI67 log-fold change.
- Pathway enrichment is exploratory and depends on the selected gene list.
- Further validation and functional experiments are needed.

## Future Work

- Verify the independent GEO2R validation results.
- Prepare publication-quality figures.
- Perform additional statistical validation.
- Investigate the functional roles of correlated genes.
- Explore experimental validation of the findings.

## Data Sources

- TCGA: https://www.cancer.gov/ccg/research/genome-sequencing/tcga
- UALCAN: https://ualcan.path.uab.edu/
- GEO dataset GSE42568: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE42568
- GEO2R: https://www.ncbi.nlm.nih.gov/geo/geo2r/
- Enrichr: https://maayanlab.cloud/Enrichr/
- PubMed: https://pubmed.ncbi.nlm.nih.gov/

## Project Status

Exploratory bioinformatics analysis completed. Figure preparation, GEO2R quality verification and research report preparation are pending.
