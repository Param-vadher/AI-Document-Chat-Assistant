<div align="center">

# 📚 AI Document Chat Assistant

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B6B?style=for-the-badge&logo=database&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

### 🎓 AIML Workshop Project - Advanced RAG Implementation

*An intelligent RAG-powered chat application that enables users to upload PDF and TXT documents and have natural conversations with an AI professor about their content.*

[Features](#-key-features) • [Installation](#-quick-start-guide) • [Usage](#-how-to-use) • [Documentation](#-project-structure) • [Contributing](#-contributing)

</div>

---

## 👨‍💻 Author

<div align="center">

**Param Vadher**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/param-vadher-b1a9b7333)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Param-vadher)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:paramvadher04@gmail.com)

📧 **Contact**: paramvadher04@gmail.com

</div>

---

## ✨ Key Features

<div align="center">

| Feature | Description |
|---------|-------------|
| 📄 **Document Upload** | Support for PDF and TXT file formats with automatic processing |
| 💬 **Intelligent Chat** | Natural conversation with AI about document content using RAG |
| 🔍 **Semantic Search** | Advanced retrieval using ChromaDB vector database & embeddings |
| 🧠 **Conversation Memory** | Maintains complete chat history for contextual responses |
| 📚 **Multi-Document Querying** | Ask questions across multiple uploaded documents simultaneously |
| 🎓 **AI Professor Mode** | Educational, explanatory responses in teaching style |
| ⚡ **FastAPI Backend** | High-performance asynchronous REST API framework |
| 🔐 **Session Management** | Secure cookie-based session handling for multiple users |

</div>

---

## 🛠️ Tech Stack

<div align="center">

| Category | Technology |
|----------|-----------|
| 🌐 **Framework** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Uvicorn](https://img.shields.io/badge/Uvicorn-2C5BB4?style=flat-square&logo=gunicorn&logoColor=white) |
| 🤖 **AI Model** | ![Google Gemini](https://img.shields.io/badge/Gemini_1.5_Flash-4285F4?style=flat-square&logo=google&logoColor=white) |
| 🔢 **Embeddings** | ![Sentence Transformers](https://img.shields.io/badge/all--MiniLM--L6--v2-FF6F00?style=flat-square&logo=huggingface&logoColor=white) |
| 💾 **Vector DB** | ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B6B?style=flat-square&logo=database&logoColor=white) |
| 📄 **PDF Processing** | ![PyMuPDF](https://img.shields.io/badge/PyMuPDF_(fitz)-40B5A4?style=flat-square&logo=adobe&logoColor=white) |
| 🎨 **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![Jinja2](https://img.shields.io/badge/Jinja2-B41717?style=flat-square&logo=jinja&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| ⚙️ **Environment** | ![Python-dotenv](https://img.shields.io/badge/.env-ECD53F?style=flat-square&logo=dotenv&logoColor=black) |

</div>

---

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- ![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white) **Python 3.8 or higher**
- 🔑 **Google Gemini API Key** - [Get it here](https://makersuite.google.com/app/apikey)
- 💻 **Basic understanding of Python and REST APIs**
- 📦 **pip** package manager

---

## 🚀 Quick Start Guide

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

---

## 📖 How to Use

### 📤 Step 1: Upload Documents

1. Click the **Upload** button in the interface
2. Select PDF or TXT files from your device
3. Wait for the success confirmation message
4. Your document is now processed and ready for queries!

### 📋 Step 2: Select Documents

1. Choose one or more documents from the dropdown menu
2. Multiple documents can be queried simultaneously
3. The AI will search across all selected documents for comprehensive answers

### 💭 Step 3: Ask Questions

1. Type your question in the chat interface
2. Receive detailed, AI-generated answers based on document content
3. Follow-up questions automatically maintain conversation context
4. Responses are formatted in a clear, educational style

### 🔄 Step 4: Continue Learning

- Ask follow-up questions to dive deeper into topics
- Switch between different documents as needed
- Clear chat history or start new sessions anytime
- Build on previous conversations for complex queries

---

## 📁 Project Structure

```
AI Document Chat Assistant/
├── 📄 app.py                  # Main FastAPI application
├── 📋 Requirements.txt        # Python dependencies
├── 🔐 .env                    # Environment variables (create this)
├── 📁 Templates/
│   └── 🌐 index.html         # Frontend interface
├── 📁 uploads/               # Uploaded documents storage
├── 📁 chroma_db/             # Vector database storage
└── 📁 __pycache__/           # Python cache files
```

---

## ⚙️ Configuration

### Document Processing Settings

| Parameter | Value | Description |
|-----------|-------|-------------|
| **Chunk Size** | 1000 characters | Size of text chunks for embedding |
| **Chunk Overlap** | 200 characters | Overlap between chunks for context continuity |
| **Embedding Model** | all-MiniLM-L6-v2 | Sentence Transformer model for embeddings |
| **Top Results** | 3 per document | Number of relevant chunks retrieved per query |

### API Configuration

| Setting | Default Value | Description |
|---------|---------------|-------------|
| **Host** | 0.0.0.0 | Server host address |
| **Port** | 8000 | Server port number |
| **Reload** | True (dev) | Auto-reload on code changes |

---

## 🌐 API Endpoints

| Method | Endpoint | Description | Status |
|--------|----------|-------------|--------|
| `GET` | `/` | Main chat interface | ✅ Active |
| `POST` | `/upload` | Upload document | ✅ Active |
| `GET` | `/documents` | List uploaded documents | ✅ Active |
| `POST` | `/chat` | Send chat message | ✅ Active |

---

## 🔒 Security & Best Practices

- 🔐 **API Keys**: Stored securely in `.env` file (never commit this file)
- 🍪 **Session Management**: HTTP-only cookies prevent XSS attacks
- ✅ **File Validation**: Uploads are sanitized and validated
- 🚫 **Git Ignore**: `.env` automatically excluded from version control
- 🔄 **Dependencies**: Regularly update packages for security patches
- 🛡️ **Input Sanitization**: All user inputs are validated and sanitized

---

## 🎯 Workshop Learning Objectives

This project was developed as part of a **One-Day AIML Workshop** covering:

<div align="center">

| Topic | Description |
|-------|-------------|
| 🏗️ **RAG Architecture** | Understanding Retrieval Augmented Generation patterns |
| 🔍 **Vector Databases** | Implementing ChromaDB for semantic search |
| 🤖 **LLM Integration** | Working with Google Gemini AI API |
| ⚡ **FastAPI Development** | Building high-performance web applications |
| 📄 **Document Processing** | Text chunking and embedding strategies |
| 💾 **Session Management** | Implementing conversation memory |
| 🚀 **Deployment** | Best practices for deploying AI applications |

</div>

---

## 🐛 Troubleshooting

<details>
<summary><b>❌ Error: GEMINI_API_KEY not found</b></summary>

**Solution:**
- Ensure `.env` file exists in the root directory
- Verify the API key is properly set in the format: `GEMINI_API_KEY=your_key_here`
- Check for any extra spaces or quotes around the key
- Restart the application after creating/modifying `.env`

</details>

<details>
<summary><b>📄 Documents not uploading</b></summary>

**Solution:**
- Verify file format is PDF or TXT only
- Check that `uploads/` directory exists and has write permissions
- Ensure file size is reasonable (< 50MB recommended)
- Try a different file to rule out corruption

</details>

<details>
<summary><b>🤖 No responses from AI</b></summary>

**Solution:**
- Verify internet connection is active
- Check Google Gemini API quota and limits
- Ensure documents are properly uploaded and selected
- Check browser console for JavaScript errors
- Verify session cookie is being set properly

</details>

<details>
<summary><b>💾 ChromaDB errors</b></summary>

**Solution:**
- Delete the `chroma_db/` folder and restart the application
- Check disk space availability
- Ensure no other process is using the database
- Verify write permissions in the project directory

</details>

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Param-vadher/AI-Document-Chat-Assistant/issues).

### How to Contribute:

1. **Fork the repository**
   ```bash
   # Click the 'Fork' button on GitHub
   ```

2. **Create your feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open a Pull Request**
   - Go to your fork on GitHub
   - Click 'New Pull Request'
   - Describe your changes in detail

### Contribution Guidelines:

- ✅ Follow PEP 8 style guidelines for Python code
- ✅ Add comments for complex logic
- ✅ Update documentation for new features
- ✅ Test your changes thoroughly before submitting
- ✅ Keep pull requests focused on a single feature/fix

---

## 📝 License

This project is licensed under the **MIT License** - feel free to use it for learning and development!

```
MIT License - see LICENSE file for details
```

---

## ⭐ Show Your Support

<div align="center">

**If you found this project helpful, please give it a ⭐ on GitHub!**

[![GitHub stars](https://img.shields.io/github/stars/Param-vadher/AI-Document-Chat-Assistant?style=social)](https://github.com/Param-vadher/AI-Document-Chat-Assistant/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Param-vadher/AI-Document-Chat-Assistant?style=social)](https://github.com/Param-vadher/AI-Document-Chat-Assistant/network/members)

</div>

---

## 📞 Contact & Support

<div align="center">

For questions, suggestions, or collaboration opportunities:

[![Email](https://img.shields.io/badge/Email-paramvadher04@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:paramvadher04@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Param_Vadher-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/param-vadher-b1a9b7333)
[![GitHub](https://img.shields.io/badge/GitHub-@Param--vadher-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Param-vadher)

**For bug reports and feature requests:** [Open an Issue](https://github.com/Param-vadher/AI-Document-Chat-Assistant/issues)

</div>

---

## 🙏 Acknowledgments

Special thanks to the amazing open-source community and tools that made this project possible:

- 🤖 **Google** - for the Gemini AI API and generative AI capabilities
- 💾 **ChromaDB Team** - for the excellent vector database solution
- 🤗 **Hugging Face** - for Sentence Transformers and ML models
- ⚡ **FastAPI Community** - for the outstanding web framework
- 📄 **PyMuPDF** - for reliable PDF processing capabilities
- 🌐 **Open Source Community** - for continuous inspiration and support

---

<div align="center">

### 💻 Built with ❤️ by Param Vadher

**AIML Workshop Project | 2026**

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)
[![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B6B?style=for-the-badge&logo=database&logoColor=white)](https://www.trychroma.com/)

---

### 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Param-vadher/AI-Document-Chat-Assistant&type=Date)](https://star-history.com/#Param-vadher/AI-Document-Chat-Assistant&Date)

---

**⭐ Don't forget to star this repository if you found it useful!**

Made with 💙 using cutting-edge AI technology

</div>
