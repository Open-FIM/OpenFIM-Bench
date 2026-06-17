# Food is Medicine Benchmark

Overview

We are building a full-detail benchmark dataset. The benchmark should evaluate whether FIM-RAG can provide accurate, grounded, safe, and context-aware nutrition guidance for people with comorbid and multimorbid health profiles.

The benchmark dataset should be built from realistic demographic, dietary, clinical, laboratory, medication, and social-context profiles.  There is no identifiable patient records so the benchmark can be freely shared, extended, and run by any contributor without privacy or IRB concerns.

The overall plan is to use:

    NHANES as the primary source for population-level demographic, dietary, social, anthropometric, laboratory, and questionnaire-derived health context.
    MIMIC as the clinical-complexity layer, especially for medically complex, medication-heavy, lab-rich, inpatient-style profiles.
    Synthetic-data methods, like synthpop (https://cran.r-project.org/web/packages/synthpop/index.html), to create statistically faithful but non-identifiable synthetic profiles.
    GenAI/LLMs to add narrative context and generate adversarial edge cases after the structured data backbone is created.

Start with the NHANES demographic and dietary extraction work. The full MIMIC dataset is currently in the process of being retrieved. Until then, the freely available 100-patient MIMIC-IV Clinical Database Demo can be used to prototype MIMIC-style extraction code.
Data access
NHANES

Use CDC/NCHS public-use NHANES data.

NHANES files are available by cycle and component:

    Demographics
    Dietary
    Examination
    Laboratory
    Questionnaire
    Limited Access Data

For this benchmark, use only public-use NHANES files.

Relevant starting points:

    NHANES main data portal:
    https://wwwn.cdc.gov/nchs/nhanes/

    NHANES dietary data page:
    https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Component=Dietary

    NHANES dietary variable list:
    https://wwwn.cdc.gov/nchs/nhanes/search/variablelist.aspx?Component=Dietary&Cycle=

Priority cycles to consider:

    NHANES 2017–March 2020 pre-pandemic
    NHANES August 2021–August 2023
    Earlier continuous NHANES cycles if needed for variable coverage or harmonization

MIMIC

The full MIMIC dataset is being retrieved separately. For now, contributors should use the MIMIC-IV Clinical Database Demo for code prototyping.

MIMIC-IV Clinical Database Demo:

    100-patient subset
    Openly available
    CSV files
    Same general schema and structure as MIMIC-IV
    Excludes free-text clinical notes
    Useful for prototyping extraction of admissions, diagnoses, labs, medications, ICU stays, and structured clinical-complexity features

MIMIC-IV Demo access page:

https://physionet.org/content/mimic-iv-demo/
Methodology

NHANES and MIMIC cannot be directly merged as if they contain the same people.

Instead,

    NHANES provides population-realistic demographic, dietary, social, and cardiometabolic context.
    MIMIC provides structured clinical-complexity patterns.
    Synthetic-data methods will need to be used to generate realistic benchmark profiles informed/guided by these data layers.
    Hybrid synthetic cases should be clearly labeled as synthetic or synthetic-hybrid profiles.
    GenAI can be used for narrative enrichment and stress-test case generation, not as a substitute for structured source data.
