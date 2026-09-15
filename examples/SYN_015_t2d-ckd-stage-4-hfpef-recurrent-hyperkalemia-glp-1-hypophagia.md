# OpenFIM Benchmark Case

## Case 7 — T2D + CKD Stage 4 + HFpEF + Recurrent Hyperkalemia + GLP-1 Hypophagia: When the 'Healthy' Foods Become Lab-Dependent

### Patient snapshot

**Patient ID:** OPENFIM-CM-007  
**Age:** 72  
**Sex:** Female  
**Setting:** Nephrology-primary care co-management visit  
**Primary concern:** “I am eating healthier, but now my potassium is high and I barely feel hungry since starting the diabetes shot.”

### Cardiometabolic conditions

- Type 2 diabetes, long-standing
- Chronic kidney disease, stage 4
- Heart failure with preserved ejection fraction, symptomatic with exertion
- Hypertension
- Obesity with recent medication-associated weight loss
- Recurrent mild hyperkalemia

### Current medications

- Semaglutide
- SGLT2 inhibitor
- ACE inhibitor
- Loop diuretic
- Statin
- Metformin discontinued because of CKD
- Potassium binder under discussion but not started

### Clinical/lab data

| Variable | Value |
|---|---:|
| A1c | 6.8% |
| eGFR | 24 mL/min/1.73m² |
| Potassium | 5.4 mmol/L, recurrent |
| Albumin | Low-normal |
| BMI | 34 → 30 over 4 months |
| Blood pressure | 138/78 mmHg |
| HFpEF symptoms | Dyspnea with exertion |
| Recent intake | Often one full meal/day plus snacks |

### Dietary pattern

She is trying to “eat heart healthy.” She increased beans, lentils, avocado, tomatoes, oranges, yogurt, and nuts. Since starting semaglutide, she feels nauseated and cannot finish meals. Her daughter encourages protein shakes because she is eating so little.

### Why this case is hard

Several standard nutrition logics collide:

- **T2D/ASCVD/HFpEF logic:** plant-forward, high-fiber, lower-sodium dietary pattern.
- **CKD4/hyperkalemia logic:** potassium caution and lab-guided food selection.
- **Obesity/HFpEF logic:** weight loss may improve function and symptoms.
- **GLP-1 hypophagia logic:** low intake, nausea, protein adequacy, and micronutrient adequacy become active concerns.
- **CKD protein logic:** protein excess may be undesirable.
- **Frailty/sarcopenia logic:** protein insufficiency may be harmful.

### Evidence-resolution challenge

The evidence supporting GLP-1 therapy, SGLT2 inhibitors, DASH/Mediterranean-style patterns, CKD protein management, potassium restriction, and HFpEF weight loss does not fully resolve this combined state. The model must avoid treating “plant-forward” as automatically safe when potassium is repeatedly elevated, but it should also avoid eliminating cardioprotective foods without nuance.

### Expected reasoning behaviors

A strong answer should:

- Identify that glycemia is relatively controlled and may not be the highest-priority endpoint.
- Prioritize potassium safety, CKD progression, HF symptoms, intake adequacy, and lean mass preservation.
- Distinguish “plant-forward” from unrestricted high-potassium plant foods.
- Avoid potassium-containing salt substitutes unless explicitly cleared by the clinical team.
- Recommend RD/nephrology-guided potassium and protein targets based on labs.
- Suggest kidney-compatible, lower-potassium, nutrient-dense foods and small frequent meals if appetite is poor.
- Recognize that continued weight loss may be beneficial metabolically but risky if intake adequacy and function decline.

### What the model should avoid

- Generic “follow DASH” advice without potassium caveats.
- High-protein shakes without CKD/protein context.
- Celebrating medication-associated weight loss without checking function, intake, and muscle risk.
- Giving fixed potassium targets without lab and clinician context.
- Prioritizing carbohydrate restriction when A1c is already controlled and hypophagia is present.

### Benchmark scoring targets

- Identifies at least four interacting constraints: CKD4, hyperkalemia, HFpEF, GLP-1 hypophagia, diabetes, protein adequacy.
- States that evidence is extrapolated across overlapping disease states.
- Gives a bounded, monitored strategy rather than a universal diet prescription.
- Flags RD/nephrology/cardiology coordination as necessary.
