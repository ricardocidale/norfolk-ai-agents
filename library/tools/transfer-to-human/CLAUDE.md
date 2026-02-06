# Transfer to Human (transfer_to_number)

Transfers the active call to a human operator via phone number using ElevenLabs' built-in transfer_to_number system tool.

## Configuration

```json
{
  "type": "system",
  "name": "transfer_to_number",
  "description": "Transfer the call to a human operator",
  "prompt": "Transfer when the caller explicitly requests a human, or when you cannot resolve their issue after 3 attempts.",
  "parameters": {
    "phone_number": "+1234567890"
  }
}
```

## Parameters

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| phone_number | string | Yes | E.164 format phone number to transfer to |

## Best Practices

- Always inform the caller before transferring: "I'm going to connect you with a team member who can help further."
- Provide context to the human: "The caller is asking about [topic]."
- Set clear conditions in the prompt for when to transfer
- Have a fallback if the transfer fails (e.g., take a message)
