# SuperConversations Methodology

The Norfolk AI SuperConversations framework is a research-backed approach to creating voice agents that build genuine rapport and achieve superior outcomes.

## Core Principles

### 43/57 Ratio
Research shows the optimal conversation ratio is **43% agent talking / 57% listening**. This means:
- Ask more questions than you give answers
- Use short, focused responses
- Let the caller fully express themselves before responding
- Avoid monologues — break long explanations into interactive segments

### The Looping Technique
A three-step pattern that ensures understanding and builds trust:

1. **Ask** — Pose a thoughtful, open-ended question
   > "What's the biggest challenge you're facing with your current setup?"

2. **Confirm** — Paraphrase their answer in your own words
   > "So if I'm hearing you correctly, the main issue is that [paraphrase]. Is that right?"

3. **Verify** — Get explicit confirmation before moving forward
   > "Great, so we're aligned on that. Let me explain how we address exactly that..."

### Deep Questions Over Surface-Level
Replace shallow questions with deeper ones:

| Surface-Level | Deep Question |
|---------------|---------------|
| "Do you like our product?" | "What would need to change for this to be a perfect fit for your team?" |
| "Any questions?" | "What's your biggest concern about moving forward?" |
| "Is the price okay?" | "How does this compare to the cost of not solving this problem?" |
| "Need anything else?" | "What would make you feel 100% confident about this decision?" |

## Implementation in Agent Prompts

Add to any agent's system prompt:
```
CONVERSATION METHODOLOGY:
Follow the SuperConversations framework:
- Maintain a 43/57 talk/listen ratio — ask more than you tell
- Use the Looping technique: Ask → Confirm back in your own words → Verify
- Prioritize deep, meaningful questions over surface-level inquiries
- After the caller speaks, briefly acknowledge what they said before responding
```
