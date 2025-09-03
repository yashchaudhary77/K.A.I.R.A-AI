# KAIRA-AI 🧠✨  
An advanced AI-powered assistant built with **FastAPI**.  
Features include document upload, text extraction (PDF, image, text), summarization, translation, and a hybrid **QA Engine** powered by **OpenAI** + **Gemini**.

---

## 🚀 Features
- 📂 **Upload Documents** → Extract text from **PDFs**, **images** (OCR), or plain text files.  
- ✂️ **Summarization** → Get concise summaries using `facebook/bart-large-cnn`.  
- 🔍 **Question Answering (QA)** → Ask questions from uploaded docs. First tries **OpenAI GPT**, falls back to **Gemini**.  
- 🌐 **Translation** → Translate between languages using **MarianMT models** (`Helsinki-NLP/opus-mt`).  
- 📜 **Clean Text** → Auto-format extracted text (line breaks, spaces).  
- ⚡ **FastAPI Backend** with CORS support → Easy to integrate with any frontend.  

---

## 🛠️ Tech Stack
- **Backend:** FastAPI, Uvicorn  
- **AI/ML Models:** Hugging Face Transformers (BART, MarianMT)  
- **OCR & Parsing:** PyMuPDF, Tesseract, pdf2image, Pillow  
- **LLMs:** OpenAI GPT, Google Gemini  
- **Others:** python-dotenv, pydantic  

---

## 📂 Project Structure
KAIRA-AI/
│
├── backend/
│ ├── app.py # Main FastAPI app
│ ├── qa.py # QA Engine (OpenAI + Gemini)
│ ├── summarizer.py # Summarization logic
│ ├── translator.py # Translation logic
│ ├── utils/
│ │ ├── pdf_reader.py # PDF/Image/Text extractor
│ │ └── text_cleaner.py # Text cleaning functions
│
├── requirements.txt # Python dependencies
├── .env # API keys (not committed to git)
└── README.md # Project documentation
