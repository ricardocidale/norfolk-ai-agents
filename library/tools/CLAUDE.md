# ElevenLabs Tools

Documentation for ElevenLabs Conversational AI tool types. These tools extend agent capabilities beyond conversation.

## Available Tool Types

- **transfer-to-human/** — Transfer call to a human operator (transfer_to_number)
- **transfer-to-agent/** — Transfer call to another AI agent (transfer_to_agent)
- **end-call/** — Programmatically end the call (end_call)

## Tool Configuration

Tools are configured in the agent's `systemTools` and `tools` fields. Each tool can have:
- **name**: Tool identifier
- **description**: What the tool does (shown to the LLM)
- **prompt**: Mini-prompt with conditions for when to use the tool
- **parameters**: JSON schema for tool parameters
- **conditions**: When the tool should be triggered
