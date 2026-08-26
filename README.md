# 🤖 Gen-AI Chatbot

![Python](https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_API-000000?style=for-the-badge&logo=groq&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-Generative_AI-brightgreen?style=for-the-badge)

## 📌 Overview
The **Gen-AI Chatbot** is a fast and responsive conversational AI application. Built using Python and Streamlit for a seamless user interface, it leverages the ultra-fast **Groq API** to process queries and generate intelligent, context-aware responses in real-time. 

## 🏗️ Architecture

Below is the data flow of how a user query is processed through the system:

```mermaid
graph TD;
    A[User Query] -->|Input| B[Streamlit UI];
    B -->|API Call| C{Groq API};
    C -->|Processing| D[Large Language Model];
    D -->|Text Generation| E[Response Output];
    E -->|Display| B;
