

```markdown
```
# Lab 3:- Build an Application to Send Chat Prompts using the Gemini Model

This lab is part of the **"Build Real World AI Applications with Gemini and Imagen"** series.

In this lab, you'll learn how to create a **chat-like application** that interacts with the **Gemini Pro** large language model to send prompts and receive intelligent responses.

---

## 🎯 Lab Objectives

- ✅ Set up and initialize **Gemini Pro** on Vertex AI
- ✅ Create a **chat-based conversation session**
- ✅ Send custom user prompts to the model
- ✅ Receive and display dynamic responses from Gemini
- ✅ Simulate a real-time chatbot experience

---

## 💡 What You'll Build

An intelligent chatbot app where users can:
- Enter natural language prompts
- Receive contextual and insightful replies
- Maintain a conversational thread using session memory

---

## 🧰 Tech Stack

| Tool              | Use Case                                 |
|-------------------|-------------------------------------------|
| Gemini Pro        | Large Language Model for text generation  |
| Vertex AI         | Platform to host and access the model     |
| Python            | Programming language                      |
| Streamlit / Flask | (Optional) Web app framework for UI       |

---

## 🚀 Step-by-Step Workflow

1. **Import Required Libraries**
   ```python
   from vertexai.preview.generative_models import GenerativeModel
   ```

2. **Initialize Gemini Model**
   ```python
   model = GenerativeModel("gemini-pro")
   chat = model.start_chat()
   ```

3. **Send User Prompt**
   ```python
   response = chat.send_message("Explain how LLMs work.")
   print(response.text)
   ```

4. **Extend the Chat**
   You can continue the conversation with follow-up questions, and the model retains context:
   ```python
   chat.send_message("Can you give an example?")
   ```

---

## 💬 Sample Prompts to Try

- “What's the future of generative AI?”
- “Summarize the importance of machine learning in healthcare.”
- “Give me 3 ideas for an AI startup.”

---

## 📦 Repository

🔗 GitHub: [Build Real World AI Applications with Gemini and Imagen](https://github.com/Yash22222/Build-Real-World-AI-Applications)

---

## ✅ Use Cases

- 🧠 AI Tutor / Educator
- 🧑‍💼 Virtual Assistant for Business
- 📜 Content & Idea Generator
- 🤖 Backend for Chatbots

---

## 🙌 Conclusion

This lab helps you understand how to use **Gemini Pro** as a conversational agent, enabling rich and dynamic interaction through text prompts. It’s a foundational building block for any **LLM-powered application**.

---


