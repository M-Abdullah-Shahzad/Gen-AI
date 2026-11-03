# Groq-Powered Chatbot

A minimal Streamlit chatbot that accepts a text question, sends it through a LangChain prompt pipeline to a Groq-hosted Llama model, and displays the generated response.

## Architecture

```text
User question → ChatPromptTemplate
→ ChatGroq (Llama 3.1) → StrOutputParser
→ Streamlit response
```

## Technology

- Python and Streamlit
- LangChain Core
- LangChain Groq integration
- Groq-hosted Llama 3.1

## Requirements

- Python 3.10+
- Groq API key
- Internet access for model inference

## Setup

1. Clone:

```bash
git clone https://github.com/M-Abdullah-Shahzad/Gen-AI.git
cd Gen-AI
```

2. Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install dependencies:

```bash
python -m pip install -r requirements.txt
```

4. Create a local .env file containing:

```env
GROQ_API_KEY=your_groq_api_key_here
```

5. Run:

```bash
streamlit run app.py
```

## Scope and limitations

This is a starter text-chat application. It does not currently implement conversation memory, document retrieval, tools, agents, user authentication, or persistent chat storage. The configured model identifier must remain available to the Groq account and API.

## Security

Never commit a populated .env file or expose your Groq API key in source code, screenshots, or logs.

## License

No license is currently declared. Contact the repository owner before redistributing this project.