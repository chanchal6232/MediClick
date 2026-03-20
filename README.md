# MediClick - Premium AI Medical Assistant

**MediClick** is a state-of-the-art medical chatbot built using Retrieval-Augmented Generation (RAG). It leverages LangChain, Pinecone, and OpenRouter (Claude 3 Haiku) to provide accurate medical information based on trusted medical literature.

## 🚀 Features
- **Premium UI**: Modern, responsive interface with glassmorphism and smooth animations.
- **RAG Powered**: Fetches context from a specialized medical knowledge base (PDF).
- **OpenRouter Integration**: Uses Claude 3 Haiku for intelligent, cost-effective responses.
- **Pinecone Vector DB**: High-performance similarity search for medical context.

---

## 🛠️ Tech Stack
- **Frontend**: HTML5, CSS3 (Custom Premium Theme), JavaScript (jQuery)
- **Backend**: Flask (Python)
- **LLM**: Claude 3 Haiku (via OpenRouter)
- **Orchestration**: LangChain
- **Vector Database**: Pinecone
- **Embeddings**: HuggingFace (MiniLM-L6-v2)

---

## 🏃 How to Run?

### Prerequisites
- Python 3.10+
- Pip (Python Package Manager)

### Step 1: Clone the Repository
```bash
git clone https://github.com/chanchal6232/Medical-Chatbot.git
cd Medical-Chatbot
```

### Step 2: Create a Virtual Environment
```bash
python -m venv venv
```

### Step 3: Activate the Virtual Environment
- **Windows**:
  ```bash
  .\venv\Scripts\activate
  ```
- **Linux/Mac**:
  ```bash
  source venv/bin/activate
  ```

### Step 4: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 5: Configure Environment Variables
Create a `.env` file in the root directory and add your credentials:
```ini
PINECONE_API_KEY="your_pinecone_key"
OPENROUTER_API_KEY="your_openrouter_key"
```

### Step 6: Store Index (Optional)
If you need to re-index the medical data from the `data/` folder:
```bash
python store_index.py
```

### Step 7: Start the Application
```bash
python app.py
```
Now, open your browser and navigate to:
`http://localhost:8080`

---

## 📁 Project Structure
- `app.py`: Main Flask application.
- `store_index.py`: Script to upsert PDF embeddings to Pinecone.
- `src/`: Core logic, helpers, and prompts.
- `static/`: Modern CSS and assets.
- `templates/`: Chat interface HTML.
- `data/`: Source medical documents (PDFs).

---

## 🤝 Contributing
Feel free to fork this project and submit pull requests for any enhancements!

## 📜 License
This project is licensed under the MIT License.
