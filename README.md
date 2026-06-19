# Cookie Cats A/B Test — Does Moving the Level Gate Improve Retention?

## Business Question
A mobile game moved its level gate from level 30 to level 40. 
Did this change improve player retention, or make it worse?

## Method
Compared two groups of players (gate_30 vs gate_40) using a 
chi-square test of independence on retention rates, and compared 
engagement levels using average and median games played.

## Findings

**Day-1 retention:** No significant difference (p = 0.075)
- gate_30: 44.8%
- gate_40: 44.2%

**Day-7 retention:** Statistically significant decrease (p = 0.0016)
- gate_30: 19.0%
- gate_40: 18.2%

**Engagement (games played):**
- gate_30: mean 52.5, median 17
- gate_40: mean 51.3, median 16

## Key Insight
The negative effect of moving the gate doesn't appear in the first 
24 hours — it only becomes statistically significant by day 7. 
This means a short A/B test window (common in fast-paced product 
teams) could easily miss this effect and ship a change that quietly 
hurts long-term retention.

## Recommendation
Keep the level gate at level 30. The later gate does not improve 
retention and shows a measurable, significant decline in players 
returning after one week.

## Data
90,189 players from a mobile game A/B test (Cookie Cats), 
split nearly evenly between two gate versions.

## Tools
Python, Pandas, SciPy (chi-square test), Matplotlib, Google Colab
