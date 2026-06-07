# TCGA-LUAD Lung Cancer Clinical Analysis
## Exploratory analysis of smoking status and clinical outcomes in lung adenocarcinoma

### Background
Lung adenocarcinoma (LUAD) is uniquely prevalent in non-smokers compared to other lung cancer subtypes. 
This analysis explores whether non-smoker LUAD patients show distinct clinical patterns — 
motivated by ongoing metabolomics research at Rajiv Gandhi Centre for Biotechnology (RGCB) 
investigating why non-smokers develop lung cancer.

### Dataset
- Source: The Cancer Genome Atlas (TCGA-LUAD)
- Portal: https://portal.gdc.cancer.gov
- Patients analysed: 2,320
- Files used: clinical.tsv, exposure.tsv

### Patient Groups
| Smoking Status | N | Avg Age at Diagnosis | Avg Pack Years |
|---|---|---|---|
| Never Smoker | 355 | 68.5 years | — |
| Former Smoker | 1,475 | 66.7 years | 36.4 |
| Current Smoker | 490 | 61.8 years | 48.8 |

### Key Findings
1. **Age at diagnosis:** Never smokers are diagnosed 6.7 years later than current smokers (68.5 vs 61.8 years), suggesting a slower or distinct biological mechanism in non-smoker lung cancer
2. **Survival rates:** Surprisingly similar across all groups (~56% alive), indicating smoking status alone does not predict survival in LUAD — pointing toward other biological drivers such as metabolic differences
3. **Gender patterns:** See chart — non-smoker LUAD shows higher female prevalence, consistent with published literature
4. **Pack years:** Current smokers show higher pack year burden (48.8) than former smokers (36.4), expected given former smokers had time to quit

### Biological Relevance
The similar survival rates despite vastly different smoking exposures suggest non-smoker LUAD 
may be driven by distinct molecular mechanisms — potentially metabolic in origin. 
This aligns with RGCB research into the metabolomes of lung cancer patients.

### Charts Generated
- chart1_distribution.png — patient counts by smoking group
- chart2_gender.png — gender breakdown by smoking group  
- chart3_age.png — age at diagnosis distributions
- chart4_packyears.png — pack years in smokers
- chart5_survival.png — survival outcomes by group

### Tools Used
Python — pandas, matplotlib, seaborn
Google Colab

### Author
Diya Jacson — Biotechnology, VIT Vellore  
Conducted during internship at Rajiv Gandhi Centre for Biotechnology, Thiruvananthapuram
