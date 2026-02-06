# Transfer to Agent (transfer_to_agent)

Transfers the active call to another AI agent within the same ElevenLabs project.

## Configuration

```json
{
  "type": "system",
  "name": "transfer_to_agent",
  "description": "Transfer the call to a specialized agent",
  "prompt": "Transfer to the sales agent when the caller expresses interest in purchasing.",
  "parameters": {
    "agent_id": "agent_abc123"
  }
}
```

## Parameters

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| agent_id | string | Yes | The ElevenLabs agent ID to transfer to |

## Best Practices

- Use descriptive trigger phrases in the prompt
- Orchestrator agents should have transfers configured for each sub-agent
- The receiving agent starts a fresh conversation — include context in the transfer if possible
- Test transfers thoroughly to ensure the correct agent receives the call
