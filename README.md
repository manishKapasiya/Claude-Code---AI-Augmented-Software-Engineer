# Claude-Code---AI-Augmented-Software-Engineer
Claude Code - AI Augmented Software Engineer with Professional Certification Notes

###Assistant Message Prefilling + Stop Sequences
This technique works by:

The user message tells Claude what to generate
The prefilled assistant message makes Claude think it already started a markdown code block
Claude continues by writing just the JSON content
When Claude tries to close the code block with ```, the stop sequence immediately ends generatio

messages = []

add_user_message(messages, "Generate a very short event bridge rule as json")
add_assistant_message(messages, "```json")

text = chat(messages, stop_sequences=["```"])

### Prompt evaluation technique


