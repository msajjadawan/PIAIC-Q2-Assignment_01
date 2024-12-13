# Open AI Parameters Understanding

## 1. Messages
   
**Purpose:** 

The messages parameter represents the conversation history between the user and the AI, formatted as a list of message objects.

**Functionality:** 

Each message object has a role (like system, user, or assistant) and content (the actual text). The system role sets the behavior, the user role specifies input from the user, and the assistant role contains AI-generated responses.

**Example:**

```json
[
  {"role": "system", "content": "You are a helpful assistant."},
  {"role": "user", "content": "What is AI?"},
  {"role": "assistant", "content": "AI stands for Artificial Intelligence."}
]
```
