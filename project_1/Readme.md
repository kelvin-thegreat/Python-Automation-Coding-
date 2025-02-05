# **Chat Assistant**

## **Overview**
This project provides multiple implementations of a chatbot using OpenAI's GPT models. The chatbot can be customized for different use cases, including financial expertise, general conversation, and idea generation. The implementations use OpenAI's API to generate responses based on user input.

## **Features**
- **[Real Estate Chat Assistant](#1-real-estate-chat-assistant-chat_assistant_websitepy)**: A chatbot specialized in real estate investment and negotiation.
- **[Custom Chat Assistant](#2-custom-chat-assistant-chat_assistantpy)**: A chatbot that allows users to define its expertise before starting the conversation.
- **[Simple ChatGPT Interface](#3-simple-chatgpt-chatgpt_simplepy)**: A minimal implementation that returns quick responses from OpenAI's API.

## **Implementations**

### **1. Real Estate Chat Assistant (`chat_assistant_website.py`)**
This implementation uses `gradio` to provide a web interface for a chatbot specialized in real estate investment and negotiation.

#### **How It Works**
- The chatbot is initialized with a system message that defines it as a **real estate expert**.
- The user provides input, which is sent to OpenAI's `gpt-3.5-turbo` model.
- The chatbot processes the response and maintains **conversation history**.
- The interface is hosted using **`gradio`** for an easy-to-use web-based chat experience.

#### **Running the Assistant**
```bash
pip install openai gradio
python chat_assistant_website.py
```

### **2. Custom Chat Assistant (`chat_assistant.py`)**
This implementation runs in the **terminal** and allows users to define the chatbot’s role dynamically.

#### **How It Works**
- The user inputs the desired **role or expertise** of the chatbot.
- A loop runs where users can chat with the assistant, and **messages are stored** to maintain context.
- The chatbot runs until the user inputs `quit()`.

#### **Running the Assistant**
```bash
pip install openai
python chat_assistant.py
```

### **3. Simple ChatGPT (`chatgpt_simple.py`)**
A minimal example that sends a single query to OpenAI's API and prints the response.

#### **How It Works**
- Uses `gpt-4o` or `gpt-3.5-turbo` to generate a **response** to a user query.
- Can be modified to accept **dynamic user input**.

#### **Running the Assistant**
```bash
pip install openai
python chatgpt_simple.py
```

## **Environment Variables**
To keep your OpenAI API key secure, use **environment variables** instead of hardcoding them:

```bash
export OPENAI_API_KEY="your-api-key"
```

Or store it in a `.env` file and load it dynamically.

## **Dependencies**
Ensure you have the required dependencies installed:
```bash
pip install openai gradio
```

## **License**
This project is **open-source** and can be modified and distributed under the terms of the **MIT License**.

## **Contributions**
Contributions are welcome! Feel free to submit **pull requests** or suggest **improvements**.

