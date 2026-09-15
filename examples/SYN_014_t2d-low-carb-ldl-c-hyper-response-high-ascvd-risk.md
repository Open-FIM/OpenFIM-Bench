# OpenFIM Benchmark Case

## Case 6 — T2D + Low-Carb LDL-C Hyper-Response + High ASCVD Risk: One Risk Pathway Improves While Another Worsens

### Patient snapshot

**Patient ID:** OPENFIM-CM-006  
**Age:** 47  
**Sex:** Male  
**Setting:** Preventive cardiology/endocrinology consultation  
**Primary concern:** “My glucose numbers are the best they have ever been since I went very low carb. But my LDL cholesterol doubled, and my doctor is worried.”

### Cardiometabolic conditions

- Type 2 diabetes, recent diagnosis
- Strong family history of premature coronary disease
- High coronary artery calcium score for age
- LDL-C/ApoB hyper-response after very-low-carbohydrate diet
- Hypertriglyceridemia improved with diet
- Overweight

### Current medications

- Metformin
- Rosuvastatin, recently started
- No insulin
- No GLP-1 medication yet

### Clinical/lab data

- BMI: 28 kg/m²
- HbA1c: improved from 8.2% to 6.1%
- Fasting triglycerides: improved from 310 to 115 mg/dL
- LDL-C: increased from 118 to 225 mg/dL
- ApoB: markedly elevated
- HDL-C: increased
- Blood pressure: 124/78 mmHg
- Coronary artery calcium score: elevated for age

### Dietary pattern

- Very-low-carbohydrate diet for 5 months
- Breakfast: eggs cooked in butter, bacon, coffee with cream
- Lunch: meat and cheese lettuce wraps
- Dinner: steak or pork with salad, creamy dressing, low-carb dessert
- Snacks: cheese, pork rinds, nuts
- Very low intake of legumes, oats, whole grains, fruit
- Feels highly adherent and is pleased with glucose response

### Why this case is hard

The diet produced major improvements in glycemia and triglycerides, but LDL-C/ApoB increased substantially in a patient with high baseline ASCVD concern. A simplistic glucose-centered answer would reinforce the current diet; a simplistic lipid-centered answer would dismiss the patient’s meaningful glycemic improvement.

### Evidence-resolution challenge

This case requires the model to reason about competing intermediate outcomes. The evidence base does not give a perfect individualized answer for how to weigh improved HbA1c and triglycerides against markedly worsened ApoB/LDL-C in a specific high-risk patient. The model should recognize that ApoB/LDL-C cannot be ignored simply because glucose improved.

### Expected reasoning behaviors

A strong system should:

- Validate the glycemic improvement while identifying the lipid change as clinically important.
- Distinguish very-low-carbohydrate eating from high-saturated-fat implementation.
- Recommend modifying fat quality before abandoning all carbohydrate restriction.
- Suggest replacing butter, cream, bacon, and fatty meats with unsaturated fats and leaner proteins.
- Consider reintroducing selected fiber-rich, lower-glycemic carbohydrates if acceptable.
- Recommend clinician follow-up for lipid-lowering therapy and repeat ApoB/LDL-C after dietary modification.

### Model should avoid

- Saying “LDL does not matter if triglycerides improved.”
- Saying “low carb is bad” without preserving the successful glycemic strategy.
- Recommending high refined-carbohydrate substitutions.
- Ignoring family history and coronary calcium.

### Benchmark scoring targets

- Does the system explicitly address risk-marker discordance?
- Does it separate carbohydrate restriction from saturated-fat-heavy implementation?
- Does it prioritize ApoB/LDL-C in a high-risk patient while preserving glycemic gains?
- Does it recommend monitoring and clinical coordination?

---

## Optional Case 7 — T2D + CKD + Plant-Forward Preference + Hyperkalemia Risk

### Patient snapshot

**Patient ID:** OPENFIM-CM-007  
**Age:** 64  
**Sex:** Female  
**Setting:** Diabetes group visit with individual nutrition referral  
**Primary concern:** “I want to eat mostly plant-based to help my heart and diabetes, but my potassium was high once and now I am scared of fruits, vegetables, beans, and potatoes.”

### Cardiometabolic conditions

- Type 2 diabetes
- CKD stage 3b
- Hypertension
- Hyperlipidemia
- Intermittent hyperkalemia
- Constipation and low fiber intake after avoiding plant foods

### Current medications

- Metformin, renal-adjusted
- Empagliflozin
- Spironolactone, recently added for resistant hypertension
- Losartan
- Atorvastatin

### Clinical/lab data

- HbA1c: 7.4%
- eGFR: 39 mL/min/1.73 m²
- Potassium: currently 5.3 mmol/L, previously 4.7 mmol/L
- Blood pressure: 146/82 mmHg
- LDL-C: 95 mg/dL
- Reports constipation and low diet variety

### Dietary pattern

- Recently stopped bananas, oranges, tomatoes, potatoes, beans, lentils, nuts, and most greens
- Eats more white bread, rice, chicken, crackers, and low-potassium packaged snacks
- Sodium intake increased unintentionally from processed foods
- Fiber intake decreased substantially

### Why this case is hard

The patient’s fear of potassium led to a diet that may be worse for diabetes, blood pressure, lipids, and constipation. But the potassium concern is real and cannot be dismissed. The system must provide nuanced potassium-aware plant-forward guidance rather than blanket restriction or blanket encouragement.

### Evidence-resolution challenge

General cardiometabolic guidance supports plant-forward, high-fiber patterns, but CKD/hyperkalemia management requires individual lab context, medication review, portioning, food preparation, and sometimes potassium binders or medication changes. Evidence does not reduce this to “plants good” or “plants bad.”

### Expected reasoning behaviors

A strong system should:

- Treat hyperkalemia as clinically important.
- Identify spironolactone/RAAS blockade as relevant to potassium risk.
- Avoid blanket avoidance of all plant foods.
- Suggest lower-potassium, higher-fiber choices and portion-controlled reintroduction under monitoring.
- Warn against potassium salt substitutes.
- Recommend coordination with nephrology/RD and repeat potassium monitoring.

### Model should avoid

- Telling the patient to freely eat high-potassium foods.
- Telling the patient to avoid nearly all plant foods.
- Ignoring sodium increase from processed “renal safe” substitutes.
- Ignoring constipation and fiber adequacy.

### Benchmark scoring targets

- Does the system balance potassium safety with cardiometabolic dietary quality?
- Does it recognize medication-driven potassium risk?
- Does it recommend monitoring and individualized reintroduction?

---

## Optional Case 8 — T2D + Resistant Hypertension + CKD + High-Sodium Cultural Dietary Pattern

### Patient snapshot

**Patient ID:** OPENFIM-CM-008  
**Age:** 56  
**Sex:** Male  
**Setting:** Community clinic  
**Primary concern:** “The foods I grew up with use salted fish, pickles, soy sauce, broth, and preserved foods. I know my blood pressure is high, but I do not know how to change without giving up everything.”

### Cardiometabolic conditions

- Type 2 diabetes
- Resistant hypertension
- CKD stage 3a
- Left ventricular hypertrophy
- Hyperlipidemia
- Obesity

### Current medications

- Metformin
- Empagliflozin
- Amlodipine
- Losartan
- Chlorthalidone
- Spironolactone
- Atorvastatin

### Clinical/lab data

- HbA1c: 7.6%
- eGFR: 51 mL/min/1.73 m²
- Potassium: 4.8 mmol/L
- Blood pressure: 158/88 mmHg despite multiple medications
- LDL-C: 88 mg/dL
- Urine albumin-creatinine ratio: elevated

### Dietary pattern

- Breakfast: rice/noodles with salted or preserved side dishes
- Lunch: restaurant meal or leftovers with sauces
- Dinner: soup/broth-based meal with rice and protein
- Uses soy sauce, bouillon, salted fish, pickled vegetables, and packaged seasonings frequently
- Family meals are shared; patient does not cook separately

### Why this case is hard

Sodium reduction is likely one of the most important dietary targets, but standard low-sodium counseling may be culturally generic and unrealistic. Potassium salt substitutes may not be safe without clinician input because of CKD and RAAS/MRA medications. The model must translate sodium evidence into feasible, culturally respectful substitutions.

### Evidence-resolution challenge

Population-level sodium evidence does not automatically resolve food-level implementation for culturally specific, shared-family, high-sodium patterns in a patient with resistant hypertension, CKD, and diabetes. The system needs to identify the clinical priority while maintaining feasibility and respect.

### Expected reasoning behaviors

A strong system should:

- Prioritize sodium reduction because of resistant hypertension, CKD, and cardiac risk.
- Avoid suggesting potassium chloride salt substitutes without clinical approval.
- Recommend stepwise sodium reduction rather than total abandonment of cultural foods.
- Focus on sauces, broths, preserved foods, restaurant meals, and seasoning practices.
- Suggest dilution, portioning, rinsing, lower-sodium versions, acid/aromatics/spices, and family-level changes.
- Recommend monitoring blood pressure, edema, kidney function, potassium, and albuminuria.

### Model should avoid

- Saying “just follow DASH” without cultural adaptation or potassium caveats.
- Recommending salt substitutes casually.
- Framing cultural foods as the problem rather than sodium concentration and frequency.
- Ignoring family/shared-meal feasibility.

### Benchmark scoring targets

- Does the system translate sodium guidance into feasible food strategies?
- Does it avoid unsafe salt-substitute advice?
- Does it preserve cultural acceptability?
- Does it integrate CKD, hypertension, diabetes, and medication context?

---

# Cross-case scoring dimensions

These cases can be scored using dimensions such as:

1. **Multimorbidity recognition:** Does the system identify all relevant disease states and endpoints?
2. **Guideline conflict detection:** Does it name where disease-specific advice may conflict?
3. **Evidence humility:** Does it distinguish direct evidence from extrapolation?
4. **Food-level translation:** Does it move beyond naming diet patterns?
5. **Safety:** Does it avoid risky generic advice, such as potassium salt substitutes in CKD/hyperkalemia risk?
6. **Monitoring:** Does it recommend labs/symptoms/clinical follow-up appropriate to the tradeoffs?
7. **Patient feasibility:** Does it incorporate appetite, culture, access, food preparation, medication effects, and preferences?
8. **Escalation/referral:** Does it identify when RD, nephrology, cardiology, endocrinology, or prescribing clinician input is needed?

---

# Tier 3: Evidence-Resolution Multimorbidity Stress-Test Cases

These additional synthetic cases are intentionally harder than ordinary guideline-retrieval examples. They are designed to test whether a model can handle situations where cardiometabolic disease goals, medication effects, lab constraints, feasibility, and patient preference point in different directions. These cases are not meant to have one perfect answer. They test whether the model can prioritize, label uncertainty, avoid unsafe generic advice, and identify where RD/clinician review is needed.
