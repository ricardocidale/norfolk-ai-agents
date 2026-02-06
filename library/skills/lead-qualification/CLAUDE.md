# Lead Qualification — BANT Framework

The BANT framework helps voice agents qualify leads efficiently by assessing four key dimensions.

## BANT Dimensions

### Budget
Understand the prospect's financial capacity and expectations.

- "What range have you allocated for this initiative?"
- "How does your team typically budget for solutions like this?"
- "Is there a specific budget you're working within?"

### Authority
Identify the decision-maker and buying process.

- "Who else on your team would be involved in evaluating this?"
- "Walk me through your typical decision-making process for something like this."
- "Besides yourself, who would need to sign off?"

### Need
Uncover the core problem and its impact.

- "What's the biggest challenge you're trying to solve?"
- "How is this issue affecting your team's productivity right now?"
- "What have you tried so far, and what worked or didn't work?"

### Timeline
Establish urgency and implementation schedule.

- "When are you looking to have a solution in place?"
- "Is there a specific event or deadline driving this timeline?"
- "What happens if this isn't resolved by [timeframe]?"

## Scoring

After qualification, score the lead:

| Score | Criteria |
|-------|----------|
| Hot (A) | All 4 BANT criteria met, decision within 30 days |
| Warm (B) | 3 of 4 criteria met, decision within 90 days |
| Cool (C) | 2 or fewer criteria met, no clear timeline |

## Implementation

Add to sales agent system prompt:
```
LEAD QUALIFICATION:
Use BANT to qualify every lead:
1. Budget — Understand their financial range
2. Authority — Identify the decision-maker
3. Need — Uncover the core problem
4. Timeline — Establish urgency
Score as Hot/Warm/Cool and adjust approach accordingly.
```
