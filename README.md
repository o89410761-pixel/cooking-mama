# Cooking Mama 👩‍🍳

**Full-day macro tracker + personalized recipe suggester** for body recomposition, weight loss, muscle gain, and performance optimization.

Stop guessing about your nutrition. Cooking Mama calculates your personalized daily calorie & macro targets, checks in at meal times, tracks what you eat, and suggests recipes tailored to your remaining macros — all without being annoying or judgmental.

## Features

✨ **Smart Goal Setting**
- Calculates personalized daily calorie needs using Harris-Benedict BMR formula
- Adjusts for your specific fitness goal (body recomposition, muscle gain, weight loss, maintenance, performance)
- Shows complete calculation breakdown with full justifications
- Gender-aware calculations (male vs. female BMR)

📊 **Daily Tracking**
- Friendly check-ins at breakfast, lunch, dinner, and snacks (via cron)
- Real-time macro accumulation as you log meals
- Supportive feedback system (never judgmental or shame-based)
- Shows remaining macros after each meal

🍽️ **Dynamic Recipe Suggestions**
- Suggests recipes based on your actual remaining daily macros
- 3–5 recipe options per meal, all within ±10% of your targets
- Shows how each recipe contributes to daily goals
- Beginner-friendly and easy-to-cook options

💪 **Sustainable Approach**
- Flexible ±5–10% daily variance (perfection is impossible)
- Weekly averaging (one day over + one day under = balanced)
- Non-restrictive, anti-shame messaging
- Monthly progress tracking

## How It Works

### Step 1: Initial Setup (One-Time)

Tell Cooking Mama about yourself:
- Gender, age, body profile (weight, height)
- Fitness goal (body recomposition, weight loss, muscle gain, etc.)
- Training frequency (how many days/week you exercise)
- Dietary preferences and cooking skill level

Cooking Mama calculates your personalized targets and shows you the math:

```
Your Personalized Targets (Body Recomposition + Performance)
===========================================================

Calculation Breakdown:

1. BMR (female, 66kg, 167cm, 22yo): 1479 kcal
2. Activity multiplier (5–6 days/week): ×1.725 = 2551 kcal TDEE
3. Goal adjustment (body recomposition): -250 cal
4. TARGET: 2301 kcal/day

Macros:
- Protein: 125g/day (preserves muscle during deficit)
- Carbs: 295g/day (fuels training + keeps energy high)
- Fat: 69g/day (supports hormones)
```

### Step 2: Daily Tracking

Cooking Mama sends friendly check-ins at fixed times:

- **08:30**: "Morning! What'd you have for breakfast?"
- **13:30**: "Lunch check-in — what'd you eat?"
- **19:30**: "Dinner time! What're you thinking?"
- **21:00**: "Any snacks today?"

You report what you ate. Cooking Mama parses it, estimates macros, and accumulates your daily total.

### Step 3: Smart Feedback

**On track?** "Nice work! You're nailing your targets!"

**Slightly over?** "Lunch ran a bit high on carbs (+15g), no worries. Just grab something lighter on carbs for dinner — plenty of room left."

**Under-fueling?** "You're running low on calories. Make sure dinner has enough fuel for your BJJ — your body needs it! 💪"

### Step 4: Recipe Suggestions

After lunch, Cooking Mama calculates exactly what you have left:

```
You've got ~1000 cal left for dinner + snacks.
If you eat dinner now (~750 cal), you'll have room for a snack later.

Here are some dinner ideas that fit perfectly:

1. Thai Curry Chicken + Jasmine Rice
   Macros: 745 cal | 42g protein | 93g carbs | 21g fat ✓

2. Teriyaki Chicken Bowl + Brown Rice
   Macros: 738 cal | 43g protein | 95g carbs | 19g fat ✓

3. Salmon & Sweet Potato + Broccoli
   Macros: 742 cal | 41g protein | 96g carbs | 20g fat ✓
```

### Step 5: Weekly Check-In

Every 7 days, Cooking Mama gives you a summary:

```
Weekly Tracking Summary (Apr 21-27)
===================================

Daily average:    2298 cal (target: 2301) ✓ ON TRACK
Protein average:  124g (target: 125g) ✓ NAILED IT
Carbs average:    293g (target: 295g) ✓ SOLID
Fat average:      69g (target: 69g) ✓ PERFECT

Weekly adherence: 94% ✨

At this consistency, you're on track for ~0.25kg fat loss/week 
with muscle maintained. That's sustainable! 💪
```

## Tone & Philosophy

**No judgment. No shame. No food police.**

Cooking Mama understands that:
- Perfect days are impossible
- Life happens (birthdays, busy days, stress)
- Weekly averaging matters more than daily perfection
- Sustainable nutrition beats restriction every time

You'll see:
- ✅ Supportive feedback, not guilt trips
- ✅ Flexible targets, not rigid rules
- ✅ Solutions-focused suggestions, not criticism
- ✅ Celebration of consistency, not punishment of slip-ups

## Installation

### As an OpenClaw Skill

```bash
# Clone this repo or download the .skill file
clawhub install cooking-mama

# Or manually copy to your skills directory
cp cooking-mama.skill ~/.openclaw/skills/
```

### Manual Setup

1. Clone this repo
2. Place it in your OpenClaw skills directory (`~/.openclaw/skills/`)
3. Restart OpenClaw
4. Start a conversation: "I want dinner ideas" or "Help me track my macros"

## Architecture

```
cooking-mama/
├── SKILL.md                          # Main skill file with workflow
└── references/
    ├── macro-optimization.md         # Formulas & calculations
    ├── tracking-patterns.md          # Feedback patterns & tone guidelines
    └── questions.md                  # Question frameworks
```

## Key References

- **`SKILL.md`** — Complete workflow, check-in system, recipe suggestions, weekly summaries
- **`macro-optimization.md`** — BMR/TDEE formulas, macro distribution, common food values
- **`tracking-patterns.md`** — Feedback patterns, messaging tone, flexibility guidelines, weekly summaries
- **`questions.md`** — Profile-building questions organized by category

## Core Concepts

### BMR & TDEE Calculation

Cooking Mama uses the **Harris-Benedict equation** to calculate your Basal Metabolic Rate (BMR):

```
Female: BMR = 447.593 + (9.247 × weight_kg) + (3.098 × height_cm) - (4.330 × age_years)
Male:   BMR = 88.362 + (13.397 × weight_kg) + (4.799 × height_cm) - (5.677 × age_years)
```

Then multiplies by your activity level to get Total Daily Energy Expenditure (TDEE):

```
Sedentary:     BMR × 1.2
Lightly active: BMR × 1.375
Moderately active: BMR × 1.55
Very active:   BMR × 1.725
Athlete:       BMR × 1.9
```

Finally, adjusts for your fitness goal:

```
Weight loss:        TDEE - 300–500 cal
Body recomposition: TDEE - 200–300 cal
Maintenance:        TDEE (no change)
Muscle gain:        TDEE + 300–500 cal
Performance:        TDEE + 100–200 cal
```

### Macro Distribution

Cooking Mama distributes your daily calories across protein, carbs, and fat based on your goal:

**Body Recomposition (your example)**:
- Protein: 1.9g per kg (preserves muscle during deficit)
- Carbs: 51% of calories (fuels training)
- Fat: 27% of calories (supports hormones)

**Muscle Gain**:
- Protein: 2.2g per kg (maximizes muscle synthesis)
- Carbs: 50% of calories (recovery)
- Fat: 25% of calories

**Weight Loss**:
- Protein: 1.6–1.8g per kg (minimizes muscle loss)
- Carbs: 40–45% of calories (moderate)
- Fat: 25–30% of calories

### Feedback Patterns

**On Track (±10%)**:
```
"Perfect! You nailed your targets today! 💪"
```

**Slight Overage (5–20% over)**:
```
"Lunch ran a bit high on carbs (+15g), no biggie. 
Just grab something lighter for dinner — plenty of room left!"
```

**Significant Overage (>20% over)**:
```
"Lunch was bigger than expected — no judgment, stuff happens! 😄
Good news: you've still got room for a solid dinner. 
Just keep it a bit lighter and you'll be back on track."
```

**Under-fueling (>15% below)**:
```
"You're running low on calories. Make sure dinner has enough fuel 
for your training — your body needs it! 💪"
```

See `references/tracking-patterns.md` for complete patterns.

## Use Cases

### Body Recomposition
Goal: Lose fat while building/maintaining muscle

```
Small calorie deficit (-250 cal/day)
High protein (1.9g per kg)
High carbs (51% of calories)
Moderate fat (27% of calories)
Result: ~0.25kg fat loss/week with muscle maintained
```

### Weight Loss
Goal: Lose weight as quickly as sustainable

```
Moderate calorie deficit (-400 cal/day)
High protein (1.6–1.8g per kg)
Moderate carbs (40–45%)
Lower fat (25–30%)
Result: ~0.5kg fat loss/week
```

### Muscle Gain
Goal: Build muscle; some fat gain acceptable

```
Small calorie surplus (+300 cal/day)
Very high protein (2.2g per kg)
High carbs (50%)
Moderate fat (25%)
Result: ~0.25–0.5kg muscle gain/week (some fat included)
```

### Maintenance
Goal: Stay where you are

```
No calorie change (TDEE)
Balanced protein (1.2g per kg)
Balanced carbs/fat
Result: Stable body composition
```

## Contributing

Have ideas to improve Cooking Mama? Issues, PRs, feedback — all welcome!

## License

MIT

---

**Made with ❤️ to help you achieve sustainable nutrition and fitness goals.**

*Cooking Mama: Because life's too short for rigid diets and shame.* 🍽️💪
