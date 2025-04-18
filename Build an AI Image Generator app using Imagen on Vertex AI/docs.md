# **Lab 2:- Build an AI Image Recognition App using Gemini on Vertex AI**

```markdown

This lab is part of the **"Build Real World AI Applications with Gemini and Imagen"** series.

In this lab, you'll learn how to create an intelligent application that understands and interprets images using **Gemini Pro Vision**, a multimodal model available on **Vertex AI**.

---

## 🎯 Lab Objectives

- ✅ Connect to Vertex AI using Python SDK
- ✅ Load the **Gemini Pro Vision** pre-trained model
- ✅ Upload and send images along with text prompts
- ✅ Extract and display the AI-generated response
- ✅ Understand how multimodal AI works in real-world applications

---

## 🧠 What You'll Build

A **Vision-based AI App** that:
- Accepts an image input (e.g. photo, chart, object)
- Uses Gemini to analyze the image
- Responds with insights based on your question

---

## 🧰 Tech Stack

| Tool              | Use Case                              |
|-------------------|----------------------------------------|
| Gemini Pro Vision | AI Model for Text + Image Understanding |
| Vertex AI         | AI Platform to run the model            |
| Python            | Programming Language                    |
| Google Cloud SDK  | Authentication and resource access      |

---

## 🚀 Steps Overview

1. **Set Up Vertex AI Studio**  
   Enable Vertex AI API and authenticate your environment.

2. **Load Gemini Vision Model in Python**  
   ```python
   from vertexai.preview.generative_models import GenerativeModel, Image
   model = GenerativeModel("gemini-pro-vision")
   ```

3. **Upload & Analyze an Image**  
   ```python
   image = Image.load_from_file("your_image.jpg")
   response = model.generate_content(["Describe this image.", image])
   print(response.text)
   ```

4. **Deploy & Extend**  
   You can integrate this into a Streamlit or Flask web app for user-friendly interaction.

---

## 💡 Real-world Use Cases

- 🔍 Business Dashboard Analyzer  
- 🧾 Invoice or Chart Interpreter  
- 📚 Visual Tutor for Students  
- 🛍️ Product Tag Generator  

---

## 📂 Repository

🔗 GitHub: [Build Real World AI Applications with Gemini and Imagen](https://github.com/Yash22222/Build-Real-World-AI-Applications)

---

## 🙌 Conclusion

By completing this lab, you’ll understand how to use **Gemini Vision** to power your image-based applications using just a few lines of code. This is a solid step toward building real-world, intelligent, multimodal GenAI apps on **Google Cloud**.

---

> **Next Lab:** Work with **Imagen** to generate images from text!
```
