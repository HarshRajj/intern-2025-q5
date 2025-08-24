# Chat Memory — CLI Chatbot
## Overview

This project implements a professional, minimal CLI chatbot using LangChain and Google Gemini 2.0 Flash. The chatbot maintains context by remembering the last 4 user-assistant turns, enabling more natural and coherent conversations.

## Features

- **Conversational Memory:** Remembers the last 4 user-assistant turns using LangChain's `ConversationBufferMemory`.
- **Google Gemini 2.0 Flash:** Utilizes the latest Gemini conversational model via LangChain integration.
- **Secure API Key Handling:** Loads your API key from a `.env` file (never hard-coded).
- **Simple CLI Interface:** Interact with the chatbot directly from your terminal.

## Getting Started

1. **Clone the repository:**
    ```bash
    git clone https://github.com/HarshRajj/intern-2025-q5.git
    cd intern-2025-q5
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Configure your API key:**
    - Create a `.env` file in the project root:
      ```
      GOOGLE_API_KEY="YOUR_API_KEY_HERE"
      ```

4. **Run the chatbot:**
    ```bash
    python main.py
    ```

## Example Conversation

```
🤖 Chatbot is ready! Type 'exit' to end the conversation.
--------------------------------------------------
You: Hello!
AI: Hello! How can I assist you today?
You: What's the weather like in Paris?
AI: I don't have real-time weather data, but Paris is often beautiful in the summer!
You: Remind me what I asked earlier.
AI: You previously asked about the weather in Paris.
You: Thanks!
AI: You're welcome! If you have more questions, feel free to ask.
You: exit
🤖 Goodbye!
```

## How it Works

- The chatbot uses LangChain's `ConversationBufferMemory` to keep track of the last 4 turns (user + assistant = 1 turn).
- Each new message is processed with the context of recent conversation history.
- Type `exit` to end the session.

## Demo

[**▶️ Run on Google Colab**](https://colab.research.google.com/drive/1jwyTm7qqOX7D8GYj9EWVZiWwOpuiipgD?usp=sharing)