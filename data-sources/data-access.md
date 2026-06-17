## Data Access

### NHANES

FIM-Bench should be built using publicly available NHANES data released by the CDC/NCHS. The objective is to maximize demographic, dietary, laboratory, examination, and health-history coverage to support realistic population generation and nutrition-focused benchmarking.

NHANES data are organized by survey cycle and component:

- Demographics
- Dietary
- Examination
- Laboratory
- Questionnaire
- Limited Access Data

### Scope

For this benchmark, **only public-use NHANES datasets should be used**. Limited-access datasets are out of scope.

### Primary Resources

- NHANES Data Portal  
  https://wwwn.cdc.gov/nchs/nhanes/

- NHANES Dietary Data Portal  
  https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Component=Dietary

- NHANES Dietary Variable Catalog  
  https://wwwn.cdc.gov/nchs/nhanes/search/variablelist.aspx?Component=Dietary&Cycle=

### Priority Survey Cycles

The following survey cycles should be prioritized:

1. **NHANES 2017–March 2020 Pre-Pandemic**
2. **NHANES August 2021–August 2023**

Additional continuous NHANES cycles may be incorporated when necessary to:

- Increase sample size
- Improve variable coverage
- Support longitudinal harmonization across survey years
- Recover variables unavailable in the priority cycles

### Data Collection Priorities

The NHANES ingestion pipeline should prioritize extraction of:

- Detailed demographic characteristics
- Dietary intake and nutrient-level variables
- Food consumption records
- Anthropometric measurements
- Clinical laboratory measurements
- Health questionnaires
- Medication usage
- Lifestyle and behavioral factors
- Comorbidity and disease indicators
- Social determinants of health

---

## MIMIC

The full MIMIC dataset is being acquired through a separate workflow. Until access is available, contributors should develop and validate ingestion code using the **MIMIC-IV Clinical Database Demo**.

### MIMIC-IV Clinical Database Demo

The demo dataset provides:

- A 100-patient subset of MIMIC-IV
- Open public access
- CSV-based data files
- Schema closely matching the full MIMIC-IV database
- Structured clinical data without free-text notes

### Intended Use

The demo dataset is sufficient for prototyping:

- Patient admission extraction
- Diagnosis and comorbidity pipelines
- Laboratory result processing
- Medication extraction
- ICU stay characterization
- Clinical trajectory reconstruction
- Structured clinical complexity feature generation

### Access

MIMIC-IV Clinical Database Demo:

https://physionet.org/content/mimic-iv-demo/

### Transition to Full MIMIC

All ingestion and feature-generation code should be written to generalize directly to the full MIMIC-IV dataset once access is available, minimizing future refactoring effort.
