# Plan: Quiz Funnel Landing Page for The 100-Day Transformation Program

## Overview
Build a premium, dark-themed quiz funnel landing page — single HTML file with inline CSS/JS. The page acts as an onboarding quiz (4 questions) that segments users into 3 product variations based on age, then shows a personalized result page with a Gumroad CTA.

## Stage 1 — Design & Build (Single Agent)
This is a focused single-page interactive experience. The vibecoding-webapp-swarm skill will handle it.

### Deliverable
One self-contained `index.html` file with:
- Inline CSS (no external stylesheets)
- Inline JavaScript (no external scripts)
- Base64-encoded logo embedded (no external images)
- All 4 quiz questions + result page
- Quiz logic mapping answers → product variation
- Correct Gumroad redirect on CTA click

### Design System
- Background: #0F0F0F
- Card background: #1A1A1A
- Card border: 1px solid #2A2A2A
- Primary text: #F0F0F0
- Secondary text: #888888
- Accent/CTA: #6BBF8A (green — fits health/fitness)
- Hover: Subtle background lightening only, no transforms
- Transitions: opacity + background-color 0.2s ease
- Progress bar: Thin horizontal, accent fill
- Typography: Clean, system fonts, fully responsive

### Quiz Structure
**Q1 (Warm-up):** Goal-related, easy engagement
**Q2 (Pain Point):** Challenge/frustration identification
**Q3 (Segmentation — KEY):** Age group → maps to variation
**Q4 (Commitment):** Readiness assessment

### Result Page
- Personalized headline + explanation referencing their answers
- "What's Included" bullets
- CTA button → correct Gumroad link
- Subtle link to other variations

### Technical Notes
- Health disclaimer in footer
- No external dependencies whatsoever
- Responsive for mobile + desktop
- Logo encoded as base64 data URI

## Skill
- `vibecoding-webapp-swarm`: For the build phase

## Execution
Single build agent will produce the complete HTML file.
