# Plan v2: Three Changes to Quiz Funnel

## Change 1: Q1 = Age Question with Image Cards
- Move age from Q3 to Q1 (still determines variation)
- Q2: Warm-up (goal), Q3: Pain Point, Q4: Commitment
- Convert 3 uploaded images (18-24.jpg, 25-39.jpg, 40-55.jpg) to base64
- Card-style UI: image on top, age label below, in a grid layout
- 3 cards side by side on desktop, stacked on mobile

## Change 2: Auto-Advance on Answer Selection
- Remove all "Next Step" / "See My Plan" buttons
- On answer click: highlight selection, wait 400ms, auto-transition to next
- Use setTimeout for the brief delay so user sees their selection
- On Q4 (last question): auto-show result page after delay

## Change 3: Remove Prices
- Remove price field from variation data
- CTA button text: "Get My 100-Day Plan" (no price)
- Update personalized text logic (Q1=age, Q2=goal, Q3=pain, Q4=commitment)

## Execution
- Convert images to base64 via Python
- Single build agent to modify the HTML with all 3 changes
- Redeploy and verify
