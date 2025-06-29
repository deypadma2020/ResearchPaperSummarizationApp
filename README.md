# ResearchPaperSummarizationApp
A Streamlit-based LLM app that lets users dynamically generate and customize research paper summaries using Anthropic's Claude model and LangChain prompt templates.

---

Here’s a clean and informative `README.md` for your project:

---

```markdown
# 📚 AI-Powered Research Paper Summarizer

This is a simple Streamlit web application that uses a Large Language Model (LLM) to summarize research papers with a customizable prompt. The app allows users to select a paper title, explanation style, and summary length to generate a clear and accurate summary with mathematical reasoning, code snippets, or analogies.

---

## 🚀 Features

- Select from well-known research papers
- Choose explanation style: Beginner-Friendly, Technical, Code-Oriented, or Mathematical
- Choose summary length: Short, Medium, or Long
- Automatically includes equations, analogies, and code examples where applicable
- Uses Anthropic’s Claude 3.5 Sonnet model via LangChain

---

## 📁 Project Structure

```

RESEARCHPAPERSUMMARIZER/
│
├── PromptTemplate/
│   └── PromptGenerator.py         # Creates and returns a dynamic prompt template
│
├── main.py                        # Streamlit app entry point
├── .env                           # Your API key goes here (not shared publicly)
├── .gitignore                     # Ignores .env, venv, cache files, etc.
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation

````

---

## 🛠️ Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/RESEARCHPAPERSUMMARIZER.git
   cd RESEARCHPAPERSUMMARIZER
````

2. **Create a virtual environment**

   ```bash
   python -m venv langchain_venv
   source langchain_venv/bin/activate  # On Windows: langchain_venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up your API key**

   * Rename `.env.example` to `.env`
   * Add your **Anthropic API key**:

     ```env
     ANTHROPIC_API_KEY=your_actual_api_key_here
     ```

---

## ▶️ Run the App

```bash
streamlit run main.py

# optionally
python -m streamlit run main.py
```

Then open `http://localhost:8501` in your browser.

---

## 🧠 Model Used

* **LLM**: [Claude 3.5 Sonnet](https://www.anthropic.com/news/claude-3-5-sonnet)
* **Framework**: [LangChain](https://www.langchain.com/)
* **Frontend**: [Streamlit](https://streamlit.io/)

---

## 📌 Customization

You can edit the prompt generation logic in `PromptTemplate/PromptGenerator.py`. The system ensures mathematical reasoning, analogies, and simplicity based on user selection.

---

## 🧾 License

This project is for educational/demo purposes. Please check the respective licenses of Anthropic, LangChain, and Streamlit for production use.

---

## 🙋‍♀️ Author

Built by Padma Dey
For contributions, bug reports, or feature requests — feel free to open an issue or fork the repo.


