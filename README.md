# Q5: Chat Memory

This repository contains the solution for Question 5 of the assignment.

## Description

A minimal CLI chatbot using LangChain and Google Gemini 2.0 Flash. The chatbot remembers the last 4 user-assistant turns using ConversationBufferMemory.

## Usage

1. **Clone the repository:**
    ```bash
    git clone https://github.com/HarshRajj/intern-2025-q5.git
    cd intern-2025-q5
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Create a `.env` file** and add your Google API key:
    ```
    GOOGLE_API_KEY="YOUR_API_KEY_HERE"
    ```

4. **Run the chatbot:**
    ```bash
    python main.py
    ```

## How it works
- The chatbot uses LangChain's ConversationBufferMemory to remember the last 4 turns.
- You can chat with the bot in your terminal. Type `exit` to quit.

## Demo

[**▶️ Run on Google Colab**](https://colab.research.google.com/drive/1jwyTm7qqOX7D8GYj9EWVZiWwOpuiipgD?usp=sharing) 