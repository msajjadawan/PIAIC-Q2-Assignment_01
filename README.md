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

**Why it’s useful:**

Helps the AI understand context by showing the conversation so far.


**Example:**

```json
[
  {"role": "system", "content": "You are a helpful assistant."},
  {"role": "user", "content": "What is AI?"},
  {"role": "assistant", "content": "AI stands for Artificial Intelligence."}
]
```


## 2. Model

This is the actual brain behind the AI. you ahve to select the proper model according to your need like 'gpt-3.5-turbo', 'gpt-4' etc

## 3.Max Completion Token

max_tokens is used to limit your answer. by providing this value you instruct the Model to generate answer and the number of token should not  increase the provided value

## 4. n

n is a parameter that instruct AI model to generate this many numbers of answers. Like if you set n=3 , it means that AI model will generate 3 possible answers and you can chose the best of them.

## 5. Stream

The stream parameter in the OpenAI Chat Completion API enables streaming responses from the model. This is useful when you want to receive tokens incrementally, which can improve user experience by showing parts of the response as they arrive rather than waiting for the entire response.

## 6. Temperature

The temperature parameter in the OpenAI Chat Completion API controls the randomness or creativity of the model's responses. By adjusting this parameter, you can fine-tune the balance between creative and deterministic outputs.

## 7. Top_p
The top_p parameter in the OpenAI API controls the "nucleus sampling" of the model's response. This parameter determines the cumulative probability of considering a subset of the most likely tokens when generating text, thereby balancing randomness and focus.

## 8. Tools
The tools parameter in the OpenAI Chat Completion API is used to integrate external tools or plugins that the model can use to enhance its functionality. These tools enable the model to perform specialized tasks or interact with external systems, such as making calculations, querying databases, fetching web results, or working with specific APIs.


