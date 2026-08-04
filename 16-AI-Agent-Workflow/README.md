# 🤖 AI Agent Workflow

An intelligent AI-powered customer service agent built with **n8n**, integrating **Google Gemini**, conversational memory, and external API tools to provide accurate and context-aware responses.

---

## 📌 Overview

This workflow demonstrates how to build an AI chatbot capable of maintaining conversation context while retrieving customer and order information through API integrations.

The AI Agent uses **Google Gemini** as its language model, **Simple Memory** for maintaining chat history, and HTTP/API tools to fetch real-time customer and order data.

---

## ✨ Features

- 💬 AI-powered customer support
- 🧠 Conversation memory
- 🤖 Google Gemini Chat Model integration
- 👤 Customer information lookup
- 📦 Order information retrieval
- 🌐 External API integration
- ⚡ Real-time responses
- 🔄 Modular AI workflow

---

## 🛠 Technologies Used

- n8n
- Google Gemini
- AI Agent Node
- Simple Memory
- HTTP Request
- REST APIs
- JSON

---

## 📂 Workflow Components

### Trigger
- When Chat Message Received

### AI Model
- Google Gemini Chat Model

### Memory
- Simple Memory

### Tools
- GetCustomers
- GetOrderData

### Output
- Context-aware AI responses with customer and order information.

---

## 🚀 How It Works

1. A user sends a chat message.
2. The workflow triggers automatically.
3. Google Gemini processes the request.
4. Conversation history is loaded from Simple Memory.
5. The AI Agent decides whether customer or order information is needed.
6. The appropriate API tool is called.
7. The retrieved data is incorporated into the AI response.
8. The final response is returned to the user.

---

## 📸 Workflow

![AI Agent](AI%20Agent.png)

---

## 🎯 Learning Outcomes

- Building AI Agents in n8n
- Integrating Large Language Models
- Using conversational memory
- Calling external APIs from AI
- Tool-based AI architecture
- Context-aware chatbot development

---

## 📄 License

This project is for educational purposes as part of the **n8n Quickstart Course**.
