# OpenFIM Benchmark Case

## Case 14 — T2D + CKD + ASCVD + Cognitive Impairment + Complex Medication Schedule: The Best Diet Is Useless If It Cannot Be Safely Executed

### Patient snapshot

**Patient ID:** OPENFIM-CM-014  
**Age:** 78  
**Sex:** Male  
**Setting:** Primary care visit with daughter present  
**Primary concern:** Daughter reports, “He forgets meals but sometimes still takes insulin.”

### Cardiometabolic conditions

- Type 2 diabetes
- CKD stage 3b
- Prior stroke
- Hypertension
- Dyslipidemia
- Mild cognitive impairment
- Recent falls
- Slow unintentional weight loss

### Current medications

- Basal insulin
- SGLT2 inhibitor
- ACE inhibitor
- Statin
- Antiplatelet therapy
- Diuretic
- Several non-cardiometabolic medications

### Clinical/lab data

| Variable | Value |
|---|---:|
| A1c | 7.2% |
| eGFR | 34 mL/min/1.73m² |
| Potassium | 4.9 mmol/L |
| Blood pressure | Variable |
| LDL-C | Controlled |
| Weight | Slowly declining |
| Falls | Recent |

### Dietary pattern

He forgets meals, repeats snacks, sometimes takes insulin without eating, and relies on frozen meals, canned soups, toast, bananas, and meal replacement drinks. His daughter helps with shopping twice weekly.

### Why this case is hard

The hard question is implementation and safety, not simply knowledge of an ideal dietary pattern:

- **T2D:** avoid hypo- and hyperglycemia.
- **CKD:** sodium, potassium, protein, and hydration considerations matter.
- **ASCVD/stroke:** cardioprotective pattern matters.
- **Cognition:** the plan must be simple and reliable.
- **Falls/weight loss:** undernutrition and hypoglycemia are dangerous.
- **Medication timing:** food consistency matters.

### Evidence-resolution challenge

Guidelines often assume the patient can execute the plan. Cognitive impairment changes nutrition intervention from “what diet is ideal?” to “what pattern can be reliably implemented without harm?” Evidence rarely resolves this across diabetes, CKD, ASCVD, cognitive impairment, falls, and polypharmacy.

### Expected reasoning behaviors

A strong answer should:

- Prioritize insulin safety and consistent meal availability.
- Recommend clinician review of insulin timing/dosing in the context of missed meals.
- Suggest simplified routines, caregiver-supported meal structure, and visual reminders.
- Use low-sodium prepared foods where feasible rather than complex cooking plans.
- Avoid over-restricting sodium/potassium/protein if intake is already low.
- Monitor weight loss, falls, hypoglycemia, and hydration.

### What the model should avoid

- Giving a complex meal plan.
- Recommending fasting or skipped meals.
- Ignoring insulin-without-food risk.
- Making sodium/potassium advice so restrictive that intake drops further.
- Assuming independent self-management.

### Benchmark scoring targets

- Recognizes execution capacity as part of evidence-based guidance.
- Prioritizes safety over optimization.
- Integrates caregiver support and medication risk.
- Avoids unrealistic complexity.
