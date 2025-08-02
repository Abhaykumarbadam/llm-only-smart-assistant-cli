# GroqCloud LLM Assistant

This is a simple command-line assistant powered by Groq's [OpenAI-compatible API](https://console.groq.com/), using the LLaMA3-70B model. The assistant provides clear, step-by-step responses to user questions and includes a basic greeting handler for casual interactions.

## Features

- Step-by-step structured answers
- Custom greetings for "hi", "hello", etc.
- Input/output logging to `interaction_logs.json`

## Requirements

- Python 3.8+
- `openai` Python package

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/groq-llm-assistant.git
   cd groq-llm-assistant
   ```

2. Install dependencies:

   ```bash
   pip install openai
   ```

3. Open `main.py` and replace this line with your actual Groq API key:

   ```python
   GROQ_API_KEY = "YOUR_GROQ_API_KEY_HERE"
   ```

## Usage

Run the assistant from the terminal:

```bash
python chatbot.py
```

You’ll see:

```
GroqCloud LLM Assistant
Type your question or 'exit' to quit
```

Start chatting! Type a question like:

```
You: Why is the sky blue?
```

To exit the session, type:

```
You: exit
```

Your conversation will be saved to a file named `interaction_logs.json`.

## Example

```
You: hi
Assistant: Hi, how can I help you today?

You: Why do we see only one side of the Moon?
Assistant: 
Step 1: The Moon is tidally locked with Earth...
...
```

## File Structure

```
.
├── main.py                    
├── level1_interaction_logs.json  # Auto-generated log file (after running)
├── README.md                  
```
