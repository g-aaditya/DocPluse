# DocPulse 🚀

**DocPulse** is an AI-powered documentation intelligence engine that reads, understands, and structures help-center content into meaningful product modules and submodules — automatically.

Built for fast analysis of large documentation websites, DocPulse crawls domain-safe URLs, extracts only what matters, and uses an LLM to infer a clean, structured module hierarchy — all delivered via a Streamlit UI or CLI.

---

## ✨ What Makes DocPulse Different?

- 🧠 AI-first understanding of documentation  
- 🌐 Domain-safe crawler with depth and page controls  
- 🧹 Noise-free content extraction  
- 🧩 Automatic module & submodule discovery  
- 🖥️ Streamlit UI  
- ⚡ CLI support  

---

## 🧭 How It Works

1. Input documentation URLs  
2. Crawl within allowed domains  
3. Extract and clean content  
4. Send content to LLM  
5. Infer modules & submodules  
6. Export structured JSON  

---

## 🏗️ Architecture

utils/  
- crawler.py  
- content_extractor.py  
- module_agent.py  

streamlit_app.py  
main.py  
config.toml  

---

## 🛠️ Tech Stack

- Python 3.9+  
- Streamlit  
- OpenAI (v1 client)  
- BeautifulSoup  
- Requests  

---

## ▶️ Usage

### Streamlit UI
```bash
streamlit run streamlit_app.py
```

### CLI
```bash
python main.py --urls https://example.com/docs
```

---

## 📦 Output

Results are saved to:
```
output/modules.json
```

---

## 📜 License

MIT License

Copyright (c) 2025 DocPulse

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
