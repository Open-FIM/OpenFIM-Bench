# OpenFIM Benchmark Case

## Case 3 — T2D + MASH/NAFLD + Hypertriglyceridemia + Obesity: Which Endpoint Comes First?

### Patient snapshot

**Patient ID:** OPENFIM-CM-003  
**Age:** 52  
**Sex:** Female  
**Setting:** Endocrinology and hepatology co-management  
**Primary concern:** “My liver doctor told me to lose weight. My diabetes doctor said reduce carbs. My lipid panel says triglycerides are high. I tried keto and my sugars improved, but my LDL went up.”

### Cardiometabolic conditions

- Type 2 diabetes
- Metabolic dysfunction-associated steatotic liver disease with suspected MASH
- Severe hypertriglyceridemia, not pancreatitis range but persistently high
- Obesity, class II
- Hypertension
- LDL-C increase during a high-saturated-fat low-carbohydrate diet

### Current medications

- Metformin
- Semaglutide
- Rosuvastatin
- Icosapent ethyl
- Amlodipine
- Losartan

### Clinical/lab data

- BMI: 38 kg/m²
- HbA1c: 7.5%, improved from 8.8% after lower-carbohydrate diet
- Fasting triglycerides: 385 mg/dL
- LDL-C: 128 mg/dL, previously 86 mg/dL
- ALT/AST: mildly elevated
- Liver stiffness/imaging suggests steatosis and possible fibrosis risk
- Blood pressure: 132/80 mmHg

### Dietary pattern

- Recently adopted low-carb eating
- Breakfast: eggs, cheese, bacon, coffee with cream
- Lunch: bunless burger, salad with creamy dressing
- Dinner: steak/chicken with non-starchy vegetables
- Snacks: cheese, nuts, low-carb packaged bars
- Very little fruit, legumes, oats, or whole grains
- High intake of saturated fat relative to baseline

### Why this case is hard

The current diet improved glycemia but worsened LDL-C. It may help triglycerides if carbohydrate quality and weight loss improve, but the implementation is high in saturated fat and low in fiber-rich foods. MASH/NAFLD guidance prioritizes weight loss and dietary quality, while diabetes guidance may emphasize carbohydrate reduction, and ASCVD prevention emphasizes atherogenic lipid lowering.

### Evidence-resolution challenge

This case exposes the difficulty of comparing dietary strategies across endpoints that move in different directions: HbA1c improves, LDL-C worsens, triglycerides remain high, liver fat needs reduction, and long-term CVD risk remains central. The evidence does not resolve this with a single universal diet label.

### Expected reasoning behaviors

A strong system should:

- Recognize that the patient experienced both benefit and harm from the current diet pattern.
- Preserve useful elements of carbohydrate quality/portion control while reducing saturated fat.
- Suggest replacing processed meats, butter, cream, and high-fat dairy with unsaturated fats and leaner proteins.
- Reintroduce selected high-fiber, lower-glycemic carbohydrates if tolerated.
- Prioritize weight loss, triglyceride reduction, liver risk reduction, and LDL-C/ApoB lowering together.
- Recommend monitoring HbA1c/CGM, fasting triglycerides, LDL-C/ApoB, liver enzymes, fibrosis markers/imaging, and weight trajectory.

### Model should avoid

- Declaring the low-carb diet a success based only on HbA1c.
- Declaring the low-carb diet a failure without preserving the glycemic benefits.
- Ignoring saturated fat quality.
- Recommending high-fructose or refined carbohydrate substitutions.
- Providing generic “Mediterranean diet” advice without addressing triglycerides and glucose.

### Benchmark scoring targets

- Does the system explicitly weigh competing endpoints?
- Does it distinguish carbohydrate amount from carbohydrate quality?
- Does it address saturated fat and LDL-C/ApoB?
- Does it recommend a modified pattern rather than a binary keto versus Mediterranean answer?

---
