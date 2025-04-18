# **Lab 4:- Build a Multi-Modal GenAI Application**


This is the final lab in the **"Build Real World AI Applications with Gemini and Imagen"** series, where you combine everything you've learned into a **fully integrated multi-modal AI application**.

---

## 🎯 Lab Objectives

- ✅ Integrate **Gemini Pro Vision** for image + text understanding  
- ✅ Use **Gemini Pro** for natural language processing and generation  
- ✅ Accept both **image inputs** and **text prompts** in a single application  
- ✅ Display and interpret **AI-generated multimodal outputs**  
- ✅ Design a user-friendly interface for interactive AI responses

---

## 💡 What You'll Build

A **Multi-Modal GenAI App** that:
- Accepts image and text inputs
- Understands visual context
- Responds using natural language
- Simulates real-world use cases like chatbots with visual input, product analysis, and virtual agents

---

## 🧰 Tech Stack

| Tool               | Purpose                                  |
|--------------------|------------------------------------------|
| Gemini Pro Vision  | Understand images + text                 |
| Gemini Pro         | Understand & generate pure text content  |
| Vertex AI          | Google Cloud's GenAI platform            |
| Python             | Backend scripting                        |
| Streamlit (optional) | Frontend UI for interactions            |

---

## 🚀 Workflow

1. **Initialize Both Models**
   ```python
   from vertexai.preview.generative_models import GenerativeModel, Image

   vision_model = GenerativeModel("gemini-pro-vision")
   text_model = GenerativeModel("gemini-pro")
   ```

2. **Load an Image and Prompt**
   ```python
   img = Image.load_from_file("sample.jpg")
   prompt = "What do you observe in this image?"
   vision_response = vision_model.generate_content([prompt, img])
   print(vision_response.text)
   ```

3. **Follow-up with Text Chat**
   ```python
   chat = text_model.start_chat()
   text_response = chat.send_message("Can you explain it more simply?")
   print(text_response.text)
   ```

---

## 🧪 Challenge Ideas

- 🤖 Build an app where users upload a product image + get marketing copy
- 📊 Analyze charts/diagrams + ask questions about trends
- 🧾 Upload receipts/invoices + extract summarized data
- 🖼️ Create a multimodal tutor that explains photos visually

---

## 📂 GitHub Repository

🔗 [Build Real World AI Applications with Gemini and Imagen](https://github.com/Yash22222/Build-Real-World-AI-Applications)

---

## 🙌 Final Thoughts

This challenge lab ties together all core concepts of **multimodal generative AI**, empowering you to build intelligent, flexible, and user-friendly applications.

Whether you're building for business, education, or creative exploration, this lab shows how to combine **text + vision** to deliver rich AI-driven experiences.

---

