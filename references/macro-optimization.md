# Macro Optimization & Fitness Goals

## Daily Macro Target Calculation

Use these formulas to estimate personalized daily macro targets based on user's body profile and fitness goal.

### Step 1: Estimate Daily Calorie Needs (TDEE) — WITH DETAILED JUSTIFICATION

**Basal Metabolic Rate (BMR)** — Harris-Benedict equation:

**For Men:**
```
BMR = 88.362 + (13.397 × weight_kg) + (4.799 × height_cm) - (5.677 × age_years)
```

**For Women:**
```
BMR = 447.593 + (9.247 × weight_kg) + (3.098 × height_cm) - (4.330 × age_years)
```

**Why this matters**: BMR is the calories your body burns just existing (breathing, heartbeat, digestion). Men have higher BMR due to greater muscle mass. The formula accounts for age (metabolism slows ~2% per decade after 30) and body size.

---

**Example Calculation (Your User: 66kg M, 167cm, 22yo)**:
```
BMR = 88.362 + (13.397 × 66) + (4.799 × 167) - (5.677 × 22)
BMR = 88.362 + 884.202 + 801.633 - 124.894
BMR = 1649 kcal
```
*Justification: This 66kg guy burns ~1649 kcal just existing. This is his baseline.*

---

### Step 2: Apply Activity Multiplier (TDEE)

Multiply BMR by activity factor based on exercise frequency/intensity:

| Activity Level | Factor | Description |
|---|---|---|
| Sedentary | 1.2 | Little/no exercise |
| Lightly active | 1.375 | 1–3 days/week light exercise |
| Moderately active | 1.55 | 3–5 days/week moderate exercise |
| Very active | 1.725 | 6–7 days/week intense exercise |
| Athlete | 1.9 | Daily intense training + recovery focus |

**Why this matters**: Exercise burns extra calories. A moderately active person burns 55% more than their BMR. A very active person burns 72.5% more.

---

**Example (Your User: Very Active — 5–6 days/week gym + cardio + BJJ)**:
```
TDEE = 1649 × 1.725 = 2844 kcal
```
*Justification: He trains hard 5–6 days/week, so he needs 72.5% more calories to fuel training + recovery.*

---

### Step 3: Adjust for Fitness Goal

Apply goal-specific calorie adjustment:

| Goal | Adjustment | Calories | Justification |
|---|---|---|---|
| **Weight Loss** | TDEE - 400 to 500 cal | 2344–2444 cal | Creates ~0.5kg/week fat loss without sacrificing muscle or energy |
| **Body Recomposition** | TDEE - 200 to 300 cal | 2544–2644 cal | Small deficit preserves muscle while slowly losing fat (sustainable) |
| **Maintenance** | TDEE (no change) | 2844 cal | Balance in = calories out, no body composition change |
| **Muscle Gain** | TDEE + 300 to 500 cal | 3144–3344 cal | Slight surplus provides energy for muscle building + recovery |
| **Performance** | TDEE + 100 to 200 cal | 2944–3044 cal | Extra fuel for intense training without excess fat gain |

**Why this matters**: 
- Fat loss requires eating less than you burn (deficit)
- Muscle gain requires eating more than you burn (surplus)
- Body recomposition uses a *small* deficit with high protein to lose fat while building/maintaining muscle
- A deficit that's too aggressive (>500 cal) causes muscle loss and fatigue

---

**Example (Your User: Body Recomposition Goal)**:
```
Target Calories = 2844 - 250 = 2594 kcal
```
*Justification: Small 250 cal deficit (~0.25kg/week fat loss) with high protein preserves muscle while slowly recomposing. Sustainable for months.*

---

### Step 4: Distribute Macros

Once you have the calorie target, break it into protein/carbs/fat based on goal:

#### **High-Protein (Muscle Gain, Weight Loss, Body Recomposition)**
```
Protein: 1.6–2.2g per kg body weight
Fat: 20–30% of total calories
Carbs: Remaining calories
```

**Example (Your User: 66kg, 2594 cal, body recomposition)**:
```
Protein: 66 × 2.0 = 132g (528 cal / 20% of total)
Fat: 2594 × 0.28 = 725 cal ÷ 9 = 81g fat
Carbs: 2594 - 528 - 725 = 1341 cal ÷ 4 = 335g carbs (52% of total)
```

*Justification:*
- **Protein 2.0g/kg**: High protein during body recomposition preserves muscle during deficit while maximizing satiety
- **28% fat**: Enough for hormone production (testosterone, growth hormone), within healthy range
- **52% carbs**: Fuels training (gym, cardio, BJJ), aids recovery, keeps energy high for performance

#### **Balanced (Maintenance, General Health)**
```
Protein: 0.8–1.2g per kg body weight
Fat: 25–35% of total calories
Carbs: Remaining calories
```

#### **Lower-Carb (Weight Loss Focus, Keto-ish)**
```
Protein: 1.4–1.8g per kg body weight
Fat: 30–40% of total calories
Carbs: 20–40% of total calories (remaining)
```

---

### Step 5: Distribute Across Meals

For 3 meals per day, allocate daily macros across breakfast, lunch, dinner + snacks:

**Standard Split** (% of daily macros):
- Breakfast: 25–30%
- Lunch: 30–35%
- Dinner: 30–35%
- Snacks/Other: 5–10%

**Example (Your User: 2594 cal, 132g protein)**:
- **Breakfast** (~650 cal, 33g protein)
- **Lunch** (~750 cal, 41g protein)
- **Dinner** (~830 cal, 42g protein)
- **Snacks** (~364 cal, 16g protein)

*Justification: Fairly even distribution across meals keeps energy and protein intake consistent throughout the day, supporting muscle protein synthesis and steady energy.*

---

## Macro Breakdown by Goal (Quick Reference)

### **Body Recomposition** (Your User's Goal)
```
Daily: 2600 cal | 132g protein | 335g carbs | 75g fat

Justification:
- Small calorie deficit (~250 cal/day = ~0.25kg fat loss/week)
- High protein (2.0g/kg) preserves muscle during deficit
- High carbs fuel training and recovery
- Moderate fat supports hormones
- Result: Slow, sustainable fat loss + muscle maintenance/growth
```

### **Weight Loss** (Aggressive)
```
Daily: 2400 cal | 110g protein | 280g carbs | 67g fat

Justification:
- Larger deficit (~450 cal/day = ~0.5kg fat loss/week)
- High protein (1.65g/kg) minimizes muscle loss
- Moderate carbs still fuel workouts
- Can be unsustainable long-term if deficit too aggressive
```

### **Muscle Gain**
```
Daily: 3100 cal | 145g protein | 395g carbs | 85g fat

Justification:
- Calorie surplus (~250 cal/day)
- Very high protein (2.2g/kg) maximizes muscle synthesis
- High carbs fuel intense training and recovery
- Modest fat gain expected; quality matters (eat nutritious surplus)
```

### **Maintenance**
```
Daily: 2844 cal | 95g protein | 365g carbs | 79g fat

Justification:
- No deficit or surplus
- Moderate protein (1.4g/kg)
- Balanced carbs/fat
- Used when already at desired body composition
```

---

## Recipe Macro Estimation

When suggesting recipes, estimate macros per serving using common reference data:

**Common foods** (per 100g unless noted):
- Chicken breast: 165 cal, 31g protein, 3.6g fat, 0g carbs
- Salmon: 206 cal, 22g protein, 13g fat, 0g carbs
- Ground beef 90/10: 176 cal, 24g protein, 8.2g fat, 0g carbs
- Egg (large): 78 cal, 6.3g protein, 5.3g fat, 0.6g carbs
- Brown rice (cooked): 112 cal, 2.6g protein, 0.9g fat, 24g carbs
- White rice (cooked): 130 cal, 2.7g protein, 0.3g fat, 28g carbs
- Sweet potato (cooked): 86 cal, 1.6g protein, 0.1g fat, 20g carbs
- Olive oil (1 tbsp/14g): 120 cal, 0g protein, 14g fat, 0g carbs
- Broccoli (100g): 34 cal, 2.8g protein, 0.4g fat, 7g carbs
- Pasta (dry, 100g): 371 cal, 13g protein, 1.1g fat, 75g carbs

**Calculation**: Sum macros of all ingredients, divide by number of servings.

**Example**:
```
Recipe: Teriyaki Chicken Bowl
- Chicken breast 200g: 330 cal, 62g protein, 7.2g fat, 0g carbs
- Brown rice 100g dry (→280g cooked): 390 cal, 9g protein, 2.5g fat, 84g carbs
- Broccoli 100g: 34 cal, 2.8g protein, 0.4g fat, 7g carbs
- Sesame oil 1 tbsp: 120 cal, 0g protein, 14g fat, 0g carbs
- Teriyaki sauce 2 tbsp: 40 cal, 0g protein, 0g fat, 10g carbs

Total: 914 cal, 73.8g protein, 24.1g fat, 101g carbs
Per serving (÷1): 914 cal | 74g protein | 24g fat | 101g carbs
```

---

## Optimization Tips

- **Protein at every meal**: Keeps user full, supports muscle recovery, enables recomposition
- **Carbs around activity**: Time carbs before/after workouts (pre-workout: 1–2 hours before; post-workout: within 2 hours)
- **Fiber**: Aim for 25–35g daily (aids digestion, satiety, health)
- **Hydration**: 3–4 liters water daily (affects performance, recovery, appetite)
- **Flexibility**: Allow ±5–10% variance from targets (100% perfection is unsustainable and unnecessary)
- **Track if serious**: If recomposition is the goal, tracking actual meals improves results significantly
- **Adjust monthly**: If not seeing progress after 3–4 weeks, adjust calories ±100–150 cal

---

## Transparency & User Communication

**Always explain the math:**

When sharing targets with the user, show them:

1. **BMR calculation** → "You burn ~1649 cal just existing"
2. **Activity multiplier** → "5–6 training days/week means you burn 72.5% more"
3. **TDEE** → "Your total daily burn is ~2844 cal"
4. **Goal adjustment** → "Small 250 cal deficit for sustainable recomposition"
5. **Final target** → "Aim for ~2594 cal, 132g protein"

**Example output**:
```
Your Personalized Targets (Body Recomposition)
==============================================

Calculation Breakdown:
- BMR (just existing): 1649 kcal
- Activity multiplier (5–6 days/week): ×1.725
- TDEE (total daily burn): 2844 kcal
- Goal adjustment (small deficit): -250 kcal
- TARGET: 2594 kcal/day

Macros:
- Protein: 132g/day (2.0g per kg | preserves muscle during deficit)
- Carbs: 335g/day (52% of calories | fuels training)
- Fat: 75g/day (28% of calories | supports hormones)

Why these numbers:
→ Small deficit ensures slow, sustainable fat loss (~0.25kg/week)
→ High protein preserves muscle while losing fat
→ High carbs fuel your gym + cardio + BJJ
→ Balanced fat supports testosterone and recovery
```

This transparency builds trust and helps users understand *why* they're eating what they eat.
