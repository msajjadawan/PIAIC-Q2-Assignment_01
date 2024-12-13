# Open AI Parameters Understanding

## 1. Messages
   
**Purpose:** 

The messages parameter represents the conversation history between the user and the AI, formatted as a list of message objects.


**How it works:**

You give the AI a list of "messages," each labeled with (role) who said it and what they said (the content - the actual text). There are three main types of roles:
   

*  System:

    Sets the tone or behavior of the AI. For example, "You are a helpful teacher."

* User: 

  Your input or question. For example, "Can you explain AI to me?"

* Assistant: 

  AI’s response (can be pre-filled if you want to include earlier responses).




**Example:**

```json
[
  {"role": "system", "content": "You are a helpful assistant."},
  {"role": "user", "content": "What is AI?"},
  {"role": "assistant", "content": "AI stands for Artificial Intelligence."}
]
```

