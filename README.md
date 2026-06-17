
# Food is Medicine Benchmark

## Overview

The **Food is Medicine (FIM) Benchmark** is a comprehensive dataset designed to evaluate whether Food-is-Medicine Retrieval-Augmented Generation (FIM-RAG) systems can deliver:

- **Accurate**
- **Grounded**
- **Safe**
- **Context-aware**

nutrition recommendations for individuals with **comorbid and multimorbid health conditions**.

The benchmark is built using **realistic, high-dimensional profiles** that integrate:

- Demographics  
- Dietary intake  
- Clinical conditions  
- Laboratory measurements  
- Medications  
- Social and behavioral context  

Importantly, the dataset contains **no identifiable patient data**, enabling:

- Open sharing  
- Reproducibility  
- Community contributions  
- No IRB or privacy constraints  

---

## Data Sources and Construction

The dataset is constructed using a hybrid approach combining real-world data sources and synthetic generation methods and includes:

- **NHANES**: Primary source for population-level demographics, diet, labs, and health context  
- **MIMIC**: Adds structured clinical complexity (comorbidities, medications, inpatient patterns)  
- **Synthetic data methods (e.g., synthpop)**: Generate statistically realistic, non-identifiable profiles  
- **GenAI / LLMs**: Provide narrative enrichment and adversarial edge cases (not a replacement for structured data)

> ⚠️ GenAI is used only for enrichment—not as a replacement for structured data sources.

---

## Development Roadmap

Current priority:

1. **NHANES extraction and harmonization**
2. **Prototype MIMIC pipelines using demo data**
3. **Integrate synthetic data generation**
4. **Add narrative and adversarial layers**

The full MIMIC dataset is currently being retrieved. Until then:

- Use the **MIMIC-IV Clinical Database Demo (100 patients)** for prototyping.

---

## Methodology

Instead, we adopt a **layered synthesis approach**:

1. **NHANES Layer**
   - Provides population-scale realism  
   - Captures diet, lifestyle, and cardiometabolic context  

2. **MIMIC Layer**
   - Provides structured clinical complexity  
   - Models comorbidity and acute care patterns  

3. **Synthetic Integration**
   - Combines both layers into realistic profiles  
   - Ensures statistical fidelity without identifiability  

4. **Hybrid Case Generation**
   - Profiles must be clearly labeled as:
     - `synthetic`
     - `synthetic-hybrid`

5. **Narrative + Adversarial Augmentation**
   - Adds real-world context (e.g., constraints, behavior)
   - Introduces failure modes for benchmarking robustness  

---

## Design Principles

- ✅ **Non-identifiable by construction**
- ✅ **Reproducible and extensible**
- ✅ **Clinically and nutritionally realistic**
- ✅ **Transparent about synthetic components**
- ✅ **Designed for stress-testing AI systems**

---

## Contribution Guidelines (Suggested)

Contributors can help with:

- NHANES data extraction and harmonization  
- MIMIC demo parsing and feature engineering  
- Synthetic data generation pipelines  
- Benchmark task design (QA, recommendations, evaluation)  
- Adversarial and edge-case scenario creation  

---

## Goal

Enable the development and evaluation of **robust, clinically safe, and context-aware Food-is-Medicine AI systems** that work reliably across:

- Diverse populations  
- Complex multimorbidity  
- Real-world constraints  
