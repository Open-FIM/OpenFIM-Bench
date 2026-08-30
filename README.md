# OpenFIM-Bench

**Population-grounded, expert-governed benchmarks for evaluating Food-is-Medicine AI**

OpenFIM-Bench is an early-stage open-source effort to develop reproducible benchmarks for evaluating whether AI-generated nutrition guidance is **appropriate, evidence-based, context-aware, and safe** for Food-is-Medicine (FIM) applications.

## Why OpenFIM-Bench?

Generative AI systems can already produce plausible nutrition recommendations. OpenFIM-Bench is being developed to help the nutrition, public-health, and AI communities investigate how AI system can go beyond and lead towards what matters, prioritize competing nutrition and health concerns, and make recommendations that fall within the range of professionally defensible nutrition judgment?

Appropriate nutrition guidance can depend on multiple interacting factors, including:

- current dietary intake;
- age, anthropometrics, and physical activity;
- laboratory measurements;
- chronic conditions and multimorbidity;
- medications and supplements, when available;
- food access and food security;
- household and socioeconomic circumstances;
- cultural context and food preferences; and
- whether the situation requires general nutrition education or professional clinical care.

Often qualified Registered Dietitian Nutritionists (RDNs) may recommend different interventions for the same person while both recommendations remain reasonable.

An AI-generated recommendation can sound plausible while overlooking an important clinical risk, applying otherwise valid nutrition advice in the wrong context, recommending unrealistic changes, or failing to recognize when professional referral is appropriate.

OpenFIM-Bench is intended to evaluate this complexity.

---

## Data Sources and Construction

The dataset is constructed using a hybrid approach combining real-world data sources and synthetic generation methods and includes:

- **NHANES**: Primary source for population-level demographics, diet, labs, and health context  
- **MIMIC**: Adds structured clinical complexity (comorbidities, medications, inpatient patterns)  
- **Synthetic data methods (e.g., synthpop)**: Generate statistically realistic, non-identifiable profiles  
- **GenAI / LLMs**: Provide narrative enrichment and adversarial edge cases (not a replacement for structured data)

The initial work focused on the **National Health and Nutrition Examination Survey (NHANES)** to construct population-grounded nutrition evaluation cases.

NHANES contains rich information collected from the same participants across domains such as:

- demographics;
- dietary recalls and nutrient intake;
- anthropometrics;
- laboratory measurements;
- health conditions;
- medications in applicable cycles;
- physical activity;
- food security; and
- socioeconomic characteristics.

These data provide valuable real-world context, OpenFIM-Bench is developing the methods and community processes needed to add evaluation layer to help answer:

- which information should be prioritized in a nutrition assessment;
- what the highest-priority nutrition problem is;
- which interventions are professionally appropriate;
- which alternative recommendations are also defensible;
- where qualified RDNs disagree; or
- which AI recommendations should be considered inappropriate or unsafe.

---

## Benchmark concept

Our current benchmark hypothesis is:

```text
Population data
      |
      v
Structured person-level nutrition case
      |
      v
Independent expert assessment
      |
      v
Agreement + acceptable variation + disagreement + safety boundaries
      |
      v
Common evaluation framework
      |
      v
Compare AI systems
```

