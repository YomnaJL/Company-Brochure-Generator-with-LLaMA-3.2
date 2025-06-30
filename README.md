
# 🧠 Company Brochure Generator with LLaMA 3.2 (via Ollama)

This project is a smart brochure generator that scrapes a company's website, extracts relevant links (like *About*, *Careers*, etc.), and uses the [LLaMA 3.2 model](https://ollama.com/library/llama3) via [Ollama](https://ollama.com/) to generate a professional company brochure in **Markdown** format.

---

## ✨ Features

- 🌐 Web scraping of company landing pages using `BeautifulSoup`
- 🔗 Intelligent link selection with LLaMA 3 via natural language prompts
- 🧾 Extraction of content from selected pages
- 📝 Brochure generation using structured markdown
- 🔄 Optional live-streaming display for notebooks (Jupyter/Colab)

---

## 📦 Requirements

- Python 3.8+
- [Ollama installed locally](https://ollama.com/download) with LLaMA 3 pulled (`ollama pull llama3`)
- Python packages:
```bash
  pip install requests beautifulsoup4 ipython
