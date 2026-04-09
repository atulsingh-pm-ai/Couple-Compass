# Couple Compass — by 30 Sundays

A pre-funnel quiz product that helps couples align on travel destinations before booking.

## Live demo
Deploy to Vercel in 60 seconds (see below).

## Product context
Built as part of a PM application to 30 Sundays. Full product brief: [30sundays.club](https://www.30sundays.club)

### Why this product?
- **JTBD addressed**: "Align on a trip before planning begins" — couples argue about destinations before any agent is involved. No tool solves this.
- **Acquisition mechanic**: Structural virality — Partner 1 cannot see results without Partner 2 completing the quiz, forcing a WhatsApp share.
- **Lead capture**: Gate placed *after* both partners finish (5–6 min invested), not at cold opt-in. Conversion is dramatically higher.
- **Zero marginal cost**: Static frontend, no backend required at launch. Leads captured via webhook to Sheets/Notion.

### Scoring logic
Each answer is tagged (beach, culture, budget-tier, etc.). Tags from both partners are aggregated and matched against destination profiles. Compatibility score is based on answer overlap across 7 dimensions.

### Tech stack
- Next.js 15 (App Router)
- TypeScript
- Tailwind CSS
- Cormorant Garamond + DM Sans (matches 30 Sundays brand tone)

## Deploy to Vercel

```bash
npm i -g vercel
vercel --prod
```

Or connect this repo to [vercel.com](https://vercel.com) for instant deploy.



## Product metrics to track (post-launch)
| Metric | Target |
|--------|--------|
| Quiz start → Partner share rate | >40% |
| Partner link → Quiz completion | >60% |
| Both done → Lead form submission | >55% |
| Lead → Consultant call booked | >25% |
| **Overall funnel** | ~6% start → quote |

---

Product designed by Atul Singh as part of 30 Sundays AI PM application.
