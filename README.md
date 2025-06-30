
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
````

---

## 🚀 How to Use

1. **Start Ollama**:

   ```bash
   ollama serve
   ```

2. **Run the script**:

   ```bash
   python brochure_generator.py
   ```

   This will:

   * Load the main page (`https://huggingface.co` by default)
   * Extract and filter links like About/Careers using LLaMA 3
   * Scrape those sub-pages
   * Generate a markdown brochure

3. **Optional (in Jupyter Notebook)**:
   To stream the result in real-time:

   ```python
   stream_brochure("HuggingFace", "https://huggingface.co")
   ```

---

## 🧠 Example Output (Markdown)

```markdown
## 🤗 Hugging Face

Hugging Face is a leader in the machine learning community. Their platform supports open collaboration between researchers and developers...

### 💼 Careers
Hugging Face is hiring! They value remote-first culture, transparency, and diversity...

### 🧑‍🤝‍🧑 Team Culture
The company believes in building ethical, open-source AI...
```

---

## 📁 Project Structure

```
📦 brochure-generator
├── brochure_generator.py      # Main script
├── README.md                  # You are here
```

---

## 🔧 Customization

You can change:

* The company name and URL
* The prompt tone (informative or humorous)
* The streaming vs non-streaming output

---

## 🛠️ Troubleshooting

* ❌ `getaddrinfo failed` → Make sure you're connected to the internet.
* ❌ `JSONDecodeError` → The LLaMA output might include extra text; we parse and clean it automatically.

---

## 📄 License

MIT License – use freely and adapt as you wish!

---

## 🤝 Credits

Made with ❤️ using:

* [Ollama](https://ollama.com/)
* [LLaMA 3](https://ollama.com/library/llama3)
* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)

```

---

Souhaites-tu que je l’inclue dans un vrai fichier `README.md` pour téléchargement ou l’adapte à un autre projet ?
```
