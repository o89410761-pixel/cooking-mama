# Tracking Patterns & Friendly Feedback

## Daily Check-In Flow

### Timing Strategy

Set up cron reminders for fixed times during the day:
- **08:00** — Breakfast check-in ("What'd you have for breakfast?")
- **13:00** — Lunch check-in ("How was lunch?")
- **19:30** — Dinner check-in ("What's for dinner?")
- **21:00** — Evening reflection ("Any snacks today?")

Users reply with what they ate. Keep it conversational, not interrogation-y.

---

## Tracking Logic

### How to Track Macros as the Day Goes

As users report their meals, **accumulate totals**:

```
Daily Target: 2301 cal | 125g protein | 295g carbs | 69g fat

Breakfast (reported): 575 cal | 31g protein | 75g carbs | 17g fat
- Cumulative: 575 cal | 31g protein | 75g carbs | 17g fat
- Remaining: 1726 cal | 94g protein | 220g carbs | 52g fat

Lunch (reported): 600 cal | 38g protein | 88g carbs | 20g fat
- Cumulative: 1175 cal | 69g protein | 163g carbs | 37g fat
- Remaining: 1126 cal | 56g protein | 132g carbs | 32g fat

Dinner (need suggestions for remaining)
- Target: ~1100 cal | ~55g protein | ~130g carbs | ~30g fat
```

---

## Friendly Feedback Patterns

### ✅ On Track
User's meal is within ±10% of target for that meal or overall progress is good.

```
"Nice! Breakfast hit your target perfectly. Great start to the day! 💪"

"Lunch was solid — you're right on track for the day."

"You crushed your protein target today — awesome work!"
```

### ⚠️ Slight Overage (5–20% over)
Don't shame. Reframe positively. Give **easy adjustments** for next meal.

```
"Lunch was a bit higher in carbs than usual (+15g), but no worries! 
Just grab something lighter on carbs for dinner — like grilled chicken + veggies. 
Still plenty of room in your daily budget."

"Protein was a touch high at lunch (+5g), but that's actually good — 
muscle building! You can dial it back slightly tomorrow if you want balance."
```

### 🚨 Significant Overage (>20% over)
Still supportive. Acknowledge it without judgment. Offer **smart next-meal strategy**.

```
"Lunch was bigger than expected — no judgment, stuff happens! 😄 
But here's the good news: you've still got room for a solid dinner. 
I'd suggest something lighter on calories (500–550 range) to keep you on track 
for your weekly average. Want some lower-cal dinner ideas?"

"You're a bit over on fat today, but that's one day out of seven. 
If you want to stay on target, just eat a leaner protein for dinner 
(fish, turkey, lean chicken). Sound good?"
```

### 📉 Under-fueling (>15% below target)
Gentle nudge. Don't force eating. Explain the "why."

```
"You're running a bit low on calories today — not bad, but make sure 
you're fueling your training! BJJ later means your body needs the fuel. 
Want a snack suggestion that fits perfectly?"

"Protein's lower today. Usually I'd say 'eat more,' but if you're not hungry, 
you don't need to force it. Just make sure dinner has solid protein for recovery. 👍"
```

---

## Dynamic Recipe Suggestions

### How to Suggest Based on Remaining Macros

Once user reports earlier meals, **calculate remaining macros** and suggest recipes that fit.

**Example**:
```
User had breakfast + lunch: 1175 cal | 69g protein | 163g carbs | 37g fat
Daily target: 2301 cal | 125g protein | 295g carbs | 69g fat

Remaining for dinner: 1126 cal | 56g protein | 132g carbs | 32g fat

Suggest recipes that hit ~1100 cal, ~55g protein, ~130g carbs.
```

**Formula**:
```
Remaining macros = Daily target - (Breakfast + Lunch reported)
Recipe suggestions must fit remaining macros ±10%
```

### Friendly Context

```
"You've got 1126 cal left for dinner + snacks. 
If you want dinner now, aim for ~1000 cal with 55g protein.
That leaves a little room for a snack later if you get hungry. 👍

Here are some ideas that fit perfectly..."
```

---

## Messaging Tone Guidelines

✅ **DO:**
- Be matter-of-fact, not preachy
- Celebrate good choices without overdoing it
- Normalize overage ("happens to everyone")
- Offer solutions, not blame
- Use humor when appropriate (😄, haha, etc.)
- Focus on what's possible next, not what went wrong

❌ **DON'T:**
- "You went over your calorie goal" (accusatory)
- "You were bad today" (judgment)
- "You need to eat less" (guilt-tripping)
- Shame language ("bloated," "damaged," "guilty pleasure")
- Overly strict tone ("You must stick to X")

### Example Corrections

**Bad**: "You exceeded your fat goal by 25g. You need to cut back."
**Good**: "Lunch was a bit higher in fat than usual — totally fine! For dinner, just pick something lighter on fat (like grilled chicken + rice) and you'll be back on track."

**Bad**: "You're not eating enough. You're sabotaging your goals."
**Good**: "You're running a bit low on calories today. Make sure dinner has enough fuel to support your BJJ — your body needs it! 💪"

**Bad**: "That's too many carbs."
**Good**: "Lunch was carb-heavy, but honestly that's great fuel for your training. For dinner, you can go lighter on carbs if you want, or keep it balanced — your call!"

---

## Handling Estimations & Uncertainty

Users won't always know exact macros. Be flexible:

```
You: "What'd you have for lunch?"
User: "Chicken and rice, not sure how much"

You: "No problem! Rough estimate: 
- Chicken: like a palm-sized piece or a small breast?
- Rice: scoop from a bowl, or a full plate?
"

[User describes portions]

You: "Gotcha, so roughly 200g chicken + 90g rice = ~730 cal, 40g protein, 92g carbs. 
Sound about right?"

User: "Yeah, sounds good"

You: [Track and proceed]
```

---

## Flexibility & Real Life

### The 80/20 Rule

Remind users that **hitting targets exactly is impossible and unnecessary**. 

```
"Here's the thing: hitting your targets perfectly every single day is impossible. 
Life happens. What matters is the trend over a week.

If today you're +200 cal, and tomorrow you're -150 cal, 
you average out to basically on-target. That's how real nutrition works."
```

### Weekly Averaging

Instead of daily perfection, track weekly trends:

```
Weekly Summary:
- Mon: +150 cal
- Tue: -100 cal
- Wed: +80 cal
- Thu: -120 cal
- Fri: ?

Your weekly average so far: +2.5% over. Basically on-point!
```

---

## When Users Miss Check-Ins

Don't be annoying. One gentle reminder, then let it go.

```
Normal flow: "Hey, missed the lunch check-in. Still on track with food?"

If they don't respond: [Don't spam. Catch them at next check-in time.]

"Dinner time! What'd you have for lunch and now?"
```

---

## Progress Feedback

### Weekly Check-In

Every 7 days, give a summary:

```
Weekly Tracking Summary
=======================

Daily average: 2298 cal (target: 2301) ✓ ON TRACK
Protein avg: 124g (target: 125g) ✓ NAILED IT
Carbs avg: 293g (target: 295g) ✓ SOLID
Fat avg: 69g (target: 69g) ✓ PERFECT

Your adherence: 94% (within ±10% of target daily average)
✨ Excellent work! This level of consistency = real results over time.

Any adjustments you want to make next week?
```

### Monthly Reflection

```
Month Summary: April
====================

Weeks tracked: 4
Weekly adherence: 92%, 89%, 95%, 91%
Average adherence: 92%

Body recomposition status (check-in):
- Feeling stronger? More energy?
- Clothes fitting differently?
- Performance in gym/BJJ improving?

At this rate (~0.25kg fat loss/week), 
you're on track for ~1kg fat loss per month with muscle maintained.
That's sustainable and realistic! 💪

Want to continue as-is, or adjust?
```

