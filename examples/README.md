# Synthetic Clinical Cases

These cases are **fully synthetic** and are intended for benchmark development, testing, and expert review. They are not real patients and should not be used for clinical care.

Each case follows a standardized structure so that cases can be reviewed and compared consistently. For several of the shorter source cases, additional synthetic details were added to match the level of context available in the more developed cases. Those additions are identified in the individual case metadata.

## Case index

| Case | Primary evaluation focus |
|---|---|
| [SYN-001 — Elena Maria: Type 2 diabetes with cardiometabolic risk and limited food access](SYN-001_elena_maria.md) | Diabetes-related dietary modification, cardiometabolic risk, affordability, cultural fit, and access to care |
| [SYN-002 — Michael R.: Metabolic dysfunction with elevated liver enzymes and severe lifestyle constraints](SYN-002_michael_r.md) | Cardiometabolic risk, possible metabolic liver disease, alcohol intake, meal timing, and feasibility for a worker with two jobs |
| [SYN-003 — Marcus Johnson: Advanced CKD with diabetes, hypertension, edema, hyperkalemia, and major social constraints](SYN-003_marcus_johnson.md) | Advanced kidney disease, competing diabetes and cardiovascular priorities, electrolyte safety, medication use, cultural fit, and escalation |
| [SYN-004 — Type 2 diabetes, CKD stage 3b, HFpEF, hypertension, and rural food insecurity](SYN-004_ckd_hfpef_diabetes.md) | Competing diabetes, CKD, and heart-failure priorities; potassium and sodium considerations; rural food access; affordability |
| [SYN-005 — Severe hypertriglyceridemia with type 2 diabetes, steatohepatitis, gout, and CKD stage 2](SYN-005_hypertriglyceridemia_nash_gout.md) | Severe hypertriglyceridemia, glycemic control, liver disease, gout, alcohol/sugar exposure, and rotating-shift feasibility |
| [SYN-006 — Type 1 diabetes, celiac disease, IBS-D, iron deficiency, and vegetarian diet](SYN-006_t1d_celiac_ibs.md) | Multiple overlapping dietary restrictions, carbohydrate consistency, micronutrient adequacy, gastrointestinal symptoms, and affordability |
| [SYN-007 — Post-bariatric frailty with coronary artery disease, CKD stage 3a, sarcopenia, and osteopenia](SYN-007_post_bariatric_frailty.md) | Frailty and malnutrition risk versus chronic disease restrictions, post-bariatric intake limitations, protein adequacy, micronutrients, and living alone |
| [SYN-008 — HIV, hyperlipidemia, osteoporosis, depression, and severe food insecurity](SYN-008_hiv_food_insecurity.md) | Food insecurity, medication interaction awareness, bone health, cardiovascular risk, unstable housing, and realistic recommendation boundaries |

## Intended benchmark use

These cases are designed to support evaluation of whether an AI system can:

1. Identify the most important nutrition-related problems from a complex person-level profile.
2. Prioritize recommendations rather than generate an exhaustive list of possible changes.
3. Modify the person’s current intake rather than replace it with a generic disease-specific meal plan.
4. Offer multiple realistic alternatives when more than one dietary strategy is reasonable.
5. Integrate relevant diagnoses, laboratory values, medications, food access, culture, work, household, and financial constraints.
6. Avoid unnecessary dietary restriction.
7. Recognize when missing information limits the safety of a recommendation.
8. Recognize when referral, escalation, or direct clinical management is warranted.
9. Separate clinical appropriateness from practical feasibility.
10. Remain within a defensible range of expert nutrition judgment rather than match one predetermined answer.
