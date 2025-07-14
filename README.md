# 📊 Form Processing Data Tool

A powerful, logic-driven Streamlit app for extracting, analyzing, and interacting with data from forms and documents. Upload images of forms, extract text using OCR, analyze with AI, chat with your data, and visualize analytics—all in one seamless interface.

---

## Features

- **Document Upload:** Upload images (JPG, PNG) of forms or documents.
- **OCR Extraction:** Extracts text from images using Mistral OCR API.
- **AI Analysis:** Analyzes extracted text for key-value pairs, completeness, and generates summaries using Llama 3 via Groq API.
- **Chatbot:** Chat with your processed data for instant Q&A and insights.
- **Analytics Dashboard:** Visualize document stats, type distribution, and processing reports.
- **Export:** Download analytics and summaries as JSON or TXT.
- **Session Management:** All data is managed in the current session for privacy and easy clearing.

---

## Tech Stack

- **Frontend:** Streamlit
- **Backend:** Python
- **OCR:** Mistral API
- **LLM:** Llama 3 via Groq API

---

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API keys:**
   - Add your API keys to `.streamlit/secrets.toml`:
     ```toml
     MISTRAL_API_KEY = "your-mistral-key"
     GROQ_API_KEY = "your-groq-key"
     ```
   - Or set them in the Streamlit Cloud secrets UI.

4. **Run the app:**
   ```bash
   streamlit run streamlit_app.py
   ```

---

## Usage

1. **Upload a document image** (JPG, PNG) in the "Document Processing" tab.
2. **Process the document** to extract text and analyze with AI.
3. **View results**: Extracted text, key-value pairs, and AI-generated summary.
4. **Chat with your data** in the "Data Chatbot" tab for instant Q&A.
5. **Explore analytics** in the "Analytics Dashboard" tab.
6. **Export** analytics or summaries as JSON/TXT for further use.
7. **Clear all data** at any time from the sidebar.

---

## Notes

- **API Keys Required:** The app will not run without valid Mistral and Groq API keys.
- **Session-based:** All data is stored in the current Streamlit session and is cleared when you use the "Clear All Data" button.
- **Image Only:** This version supports image uploads (JPG, PNG). For PDF/DOCX/text support, see future plans.
- **No Database:** This version does not use a persistent database; all processing is in-memory for privacy and simplicity.

---

## Future Improvements

- Support for PDF, DOCX, and text file uploads.
- Persistent user/session storage and authentication.
- More robust error handling and logging.
- Multi-user support and production-ready data management.

---

## License

MIT License

---

**Built with ❤️ using Streamlit, Mistral OCR, and Groq Llama 3.** 
