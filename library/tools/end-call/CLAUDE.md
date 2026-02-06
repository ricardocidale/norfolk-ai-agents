# End Call (end_call)

Programmatically ends the active call. Used for graceful call termination based on conditions.

## Configuration

```json
{
  "type": "system",
  "name": "end_call",
  "description": "End the call gracefully",
  "prompt": "End the call after the caller confirms they have no more questions, or after saying goodbye."
}
```

## When to Use

- Caller has confirmed resolution: "No, that's everything. Thank you!"
- Caller says goodbye: "Thanks, bye!"
- Maximum conversation length reached
- Abusive or inappropriate caller (after warning)
- No response after extended silence

## Best Practices

- Always give a farewell message before ending: "Thank you for calling! Have a great day. Goodbye."
- Don't end calls abruptly — wait for natural conversation endings
- Combine with `endCallAfterSilence` setting for automatic timeout
- Log the end reason for analytics
