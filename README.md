# 💬 Streamlit Chatbot using Google Gemini API

This is a simple chatbot web application built using **Streamlit** and **Google's Generative AI (Gemini API)**. The chatbot takes user input and returns a conversational response using Gemini's `models/gemini-1.5-flash` model.

---

## 🚀 Features

* Simple, interactive web interface using Streamlit
* Seamless integration with Google Gemini API
* Chat history maintained across the session
* Loading spinner during response generation

---

## 🛠️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/streamlit-gemini-chatbot.git
   cd streamlit-gemini-chatbot
   ```

2. **Install the required packages**
   Make sure you have Python 3.7 or above.

   ```bash
   pip install streamlit google-generativeai
   ```

3. **Set your API Key**
   Replace the `api` variable in `chatbot.py` with your [Google Generative AI API Key](https://makersuite.google.com/app/apikey).

---

## 📂 File Structure

```
├── chatbot.py       # Main Streamlit app
├── README.md        # Project documentation
```

---

## ▶️ Running the App

```bash
streamlit run chatbot.py
```

Open the URL that appears in the terminal (usually [http://localhost:8501](http://localhost:8501)) to use the chatbot.

---

## 🧠 How It Works

* User enters a message via `st.chat_input`
* Message is sent to Gemini's `models/gemini-1.5-flash`
* The response is generated and displayed using Streamlit’s `st.chat_message`
* Session state (`st.session_state.messages`) is used to maintain chat history

---

## ⚠️ Notes

* Do **not** expose your API key in production environments. Use environment variables or secret management.
* The Gemini API usage may be subject to quotas and rate limits.

---
