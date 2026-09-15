# OpenFIM Benchmark Case

## Case 11 — T2D + Resistant Hypertension + CKD + Gout + Culturally High-Sodium Diet: Sodium Advice Is Not Enough

### Patient snapshot

**Patient ID:** OPENFIM-CM-011  
**Age:** 59  
**Sex:** Male  
**Setting:** Primary care visit for uncontrolled blood pressure  
**Primary concern:** “Everyone tells me to stop salt, but this is how my family cooks.”

### Cardiometabolic conditions

- Type 2 diabetes
- Resistant hypertension
- CKD stage 3a with albuminuria
- Gout/hyperuricemia
- Obesity
- Dyslipidemia

### Current medications

- Metformin
- SGLT2 inhibitor
- ACE inhibitor
- Thiazide-like diuretic
- Calcium channel blocker
- Allopurinol
- Statin

### Clinical/lab data

| Variable | Value |
|---|---:|
| A1c | 7.6% |
| eGFR | 48 mL/min/1.73m² |
| Uric acid | High |
| Blood pressure | 158/92 mmHg on 3 medications |
| Potassium | Normal-high |
| Albuminuria | Present |
| BMI | 33 |

### Dietary pattern

Meals often include salted soups, pickled vegetables, cured meats, white rice, sweet tea, fried snacks, and large evening portions. Food is prepared for the household, and he is not the main cook.

### Why this case is hard

A generic sodium-reduction message misses the implementation challenge:

- **Resistant hypertension:** sodium reduction is clinically important.
- **CKD:** kidney protection and sodium control matter.
- **T2D:** glycemic load and meal timing matter.
- **Gout:** purines, alcohol, fructose, and weight loss may matter.
- **Medication context:** potassium salt substitutes may be risky with CKD/ACE inhibitor use.
- **Cultural/family context:** the plan must fit shared meals.

### Evidence-resolution challenge

Evidence supports sodium reduction for blood pressure, but it does not fully specify culturally tailored substitutions that also account for CKD, diabetes, gout, medication interactions, and household food roles. The model must reason from principles without pretending one generic pattern solves everything.

### Expected reasoning behaviors

A strong answer should:

- Identify high-impact sodium sources in the current pattern.
- Offer culturally plausible lower-sodium modifications rather than unfamiliar replacement diets.
- Avoid casual potassium chloride salt-substitute recommendations.
- Address sweetened beverages and refined carbohydrate load.
- Discuss gout-relevant choices without unnecessarily banning entire food groups.
- Include household cook/family-level implementation.

### What the model should avoid

- Simply saying “follow DASH.”
- Recommending potassium chloride salt substitutes without CKD/medication caveats.
- Over-restricting all meats or legumes without nuance.
- Ignoring family food context.
- Prescribing unfamiliar foods as the primary solution.

### Benchmark scoring targets

- Separates sodium, potassium, gout, glycemia, and culture/feasibility constraints.
- Gives implementable substitutions.
- Avoids unsafe salt-substitute advice.
- Acknowledges evidence gaps in culturally specific multimorbidity nutrition guidance.
