# 📚 AI Document Chat Assistant

### 🎓 AIML Workshop Project - One Day Workshop

🤖 An intelligent RAG-powered chat application that enables users to upload PDF and TXT documents, then have natural conversations with an AI professor about their content. Features multi-document querying, semantic search via ChromaDB, conversation memory, and contextual responses using Google Gemini AI.

---

## 👨‍💻 Author

**Param Vadher**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/param-vadher-b1a9b7333)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Param-vadher)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:paramvadher04@gmail.com)

📧 **Contact**: paramvadher04@gmail.com

---

## ✨ Key Features

- 📄 **Document Upload** - Support for PDF and TXT file formats
- 💬 **Intelligent Chat** - Natural conversation with AI about document content
- 🔍 **Semantic Search** - Powered by ChromaDB vector database and Sentence Transformers
- 🧠 **Conversation Memory** - Maintains chat history for contextual responses
- 📚 **Multi-Document Querying** - Ask questions across multiple uploaded documents
- 🎓 **AI Professor Mode** - Responses in educational, explanatory style
- ⚡ **FastAPI Backend** - High-performance asynchronous web framework
- 🔐 **Session Management** - Secure cookie-based session handling

## 🛠️ Tech Stack
| Category | Technology |
|----------|-----------|
| 🌐 **Framework** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white) |
| 🤖 **AI Model** | ![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=flat&logo=google&logoColor=white) |
| 🔢 **Embeddings** | ![Sentence Transformers](https://img.shields.io/badge/Sentence_Transformers-FF6F00?style=flat&logo=python&logoColor=white) |
| 💾 **Vector DB** | ![ChromaDB](https://img.shields.io/badge/ChromaDB-000000?style=flat&logo=database&logoColor=white) |
| 📄 **PDF Processing** | ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-40B5A4?style=flat&logo=adobe&logoColor=white) |
| 🎨 **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![Jinja2](https://img.shields.io/badge/Jinja2-B41717?style=flat&logo=jinja&logoColor=white) |
| ⚙️ **Environment** | ![Python-dotenv](https://img.shields.io/badge/.env-ECD53F?style=flat&logo=.env&logoColor=black) |
| 🐍 *Prerequisites

- ![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
- 🔑 Google Gemini API Key ([Get it here](https://makersuite.google.com/app/apikey))
- 💻 Basic understanding of Python and REST APIs

- Python 3.8+
- Google Gemini API Key
Quick Start Guide

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Param-vadher/AI-Document-Chat-Assistant.git
cd "AI Document Chat Assistant"
   ```
### 2️⃣ Install Dependencies
```bash
pip install -r Requirements.txt
```

### 3️⃣ Configure Environment Variables

Create a `.env` file in the root directory:
```env
GEMINI_API_KEY=your_gemini_api_key_here
```

> 💡 **Tip**: Get your Gemini API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### 4️⃣ Run the Application

**Option 1: Using Python**
```bash
python app.py
```

**Option 2: Using Uvicorn**
```bash
uvicorn app:app --reload
```

### 5️⃣ Access the Application

Open your browser and navigate to:
```
🌐 http://localhost:8000
```
How to Use

### Step 1: 📤 Upload Documents
- Click the **Upload** button
- Select PDF or TXT files from your device
- Wait for the success confirmation message

### Step 2: 📋 Select Documents
- Choose one or more documents from the dropdown menu
- Multiple documents can be queried simultaneously for comprehensive answers

### Step 3: 💭 Ask Questions
- Type your question in the chat interface
- Receive detailed AI-generated answers based on document content
- Follow-up questions automatically maintain conversation context

### Step 4: 🔄 Continue Learning
- Ask follow-up questions to dive deeper
- Switch between different documents as needed
- Clear history or start new sessions anytime
3. **Ask Questions**
   - Type your question in the chat interface
   - Receive AI-generated answers based on document content
   - Follow-up questions maintain conversation context

## 📁 Project Structure

```
AI Document Chat Assistant/
├── app.py                  # Main FastAPI application
├── Requirements.txt        # Python dependencies
├── .env                    # Environment variables (create this)
├── Templates/
│   └── index.html         # Frontend interface
├── uploads/               # Uploaded documents storage
├── chroma_db/             # Vector database storage
└── __pycache__/           # Python cache files
```

## 🔧 Configuration

### Document Processing
- **Chunk Size**: 1000 characters
- **Chunk Overlap**: 200 characters Status |
|--------|----------|-------------|--------|
| `GET` | `/` | Main chat interface | ✅ Active |
| `POST` | `/upload` | Upload document | ✅ Active |
| `GET` | `/documents` | List uploaded documents | ✅ Active |
| `POST` | `/chat` | Send chat message | ✅ Activ

## 🌐 API Endpo& Best Practices

- 🔐 API keys are stored in `.env` file (**never commit this file**)
- 🍪 Session IDs are stored in HTTP-only cookies
- ✅ File uploads are sanitized and validated
- 🚫 Add `.env` to your `.gitignore` file
- 🔄 Regularly update dependencies for security patches
| POST | `/upload` | Upload document |
| GET | `/documents` | List uploaded documents |
| POST | `/chat` | Send chat message |
🎯 Workshop Learning Objectives

This project was developed as part of a **One-Day AIML Workshop** covering:

- ✅ Understanding RAG (Retrieval Augmented Generation) architecture
- ✅ Implementing vector databases for semantic search
- ✅ Integrating Google Gemini AI for intelligent responses
- ✅ Building FastAPI web applications
- ✅ Document processing and text chunking strategies
- ✅ Session management and conversation memory
- ✅ Deploying AI-powered applications

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Param-vadher/AI-Document-Chat-Assistant/issues).

### How to Contribute:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the **MIT License** - feel free to use it for learning and development!

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐ on GitHub!
## 🤝 Contact & Support

For questions, suggestions, or collaboration opportunities:

- 📧 Email: [paramvadher04@gmail.com](mailto:paramvadher04@gmail.com)
- 💼 LinkedIn: [Param Vadher](https://www.linkedin.com/in/param-vadher-b1a9b7333)
- 🐙 GitHub: [@Param-vadher](https://github.com/Param-vadher)

For bug reports and feature requests, please [open an issue](https://github.com/Param-vadher/AI-Document-Chat-Assistant/issues).

---

## 🙏 Acknowledgments

- Google for Gemini AI API
- ChromaDB team for the vector database
- Hugging Face for Sentence Transformers
- FastAPI community for the excellent framework

---

<div align="center">

### Built with ❤️ by Param Vadher

**AIML Workshop Project | 2024**

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)

**⭐ Star this repo if you find it useful!**

</div>the MIT License.

## 🐛 Troubleshooting

### Common Issues

**Error: GEMINI_API_KEY not found**
- Ensure `.env` file exists in the root directory
- Verify the API key is properly set

**Documents not uploading**
- Check file format (PDF or TXT only)
- Ensure `uploads/` directory has write permissions

**No responses from AI**
- Verify internet connection
- Check Gemini API quota/limits
- Ensure documents are properly uploaded and selected

## 📧 Support

For issues and questions, please open an issue in the repository.

---

Built with ❤️ using FastAPI and Google Gemini AI
