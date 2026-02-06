# Custom Commands — Norfolk AI Voice Agent Factory

## /create-agent

Create a new agent folder with CLAUDE.md configuration.

### Steps:
1. Navigate to the target project: `clients/{client}/projects/{project}/agents/`
2. Create a new folder with the agent's sanitized name
3. Create `CLAUDE.md` inside with the following sections:
   - Title with agent name and code
   - System Prompt (most important — place first)
   - First Message
   - Voice Configuration (voiceId, TTS model, stability, similarity)
   - LLM Configuration (provider, model, temperature)
   - Personality (gender, age, mood, tone, traits)
   - Tools & Transfers
4. Create a `knowledge/CLAUDE.md` subfolder for knowledge base documents
5. If this is a sub-agent, place it under `agents/{parent}/team/{name}/`

---

## /optimize-prompt

Improve an agent's system prompt for better conversation quality.

### Checklist:
1. Open the agent's CLAUDE.md
2. Review the System Prompt section
3. Check for:
   - Clear role definition in the first sentence
   - Specific behavioral guidelines (do's and don'ts)
   - Conversation flow structure (greeting → discovery → action → closing)
   - Guardrails and boundaries
   - Error handling instructions
4. Apply SuperConversations methodology:
   - Add 43/57 ratio instruction
   - Include Looping technique (Ask → Confirm → Verify)
   - Replace surface-level questions with deep questions
5. Ensure the prompt is under 4000 characters for optimal performance

---

## /add-transfer-target

Add a new transfer destination to an agent.

### Steps:
1. Open the agent's CLAUDE.md
2. Find the Tools & Transfers section
3. Add a new entry under Transfer to Agents:
   - Agent ID: The ElevenLabs agent ID of the target
   - Trigger Phrase: When should this transfer happen
   - Conditions: Any prerequisites for the transfer
4. Update the System Prompt to include routing instructions for the new target
5. Test the transfer flow end-to-end

---

## /review-agent

Checklist for reviewing agent configuration quality.

### Review Checklist:
- [ ] System prompt is clear, specific, and under 4000 characters
- [ ] First message is welcoming and sets expectations
- [ ] Voice ID is configured and matches the agent's personality
- [ ] TTS model is set to eleven_turbo_v2_5 for low latency
- [ ] Stability is between 0.5 and 0.7
- [ ] Speaker boost is disabled for lower latency
- [ ] All transfer targets have valid agent IDs
- [ ] Transfer conditions are clearly defined in the system prompt
- [ ] Dynamic variables have sensible defaults
- [ ] Language settings match the project's language priorities
- [ ] Max duration is set appropriately for the agent's purpose
- [ ] End-after-silence is configured (recommended: 10-15s)
- [ ] Quality score is above 70/100
- [ ] Knowledge base documents are relevant and up-to-date
