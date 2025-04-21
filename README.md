# 🔍 ReconAI — AI-Enhanced OSINT Recon Tool

> A powerful Python tool that automates OSINT data collection and enhances it with AI for faster, smarter recon.

## 🚀 Features

- 🌐 Domain & Subdomain enumeration
- 🕵️ Social media profile scraper (LinkedIn, GitHub, Twitter)
- 🧠 AI-based threat vector prediction
- 📊 Named Entity Recognition (NER)
- 📄 Generates clean, structured PDF/Markdown reports
- 🖥️ Optional GUI with Streamlit

## 🛠️ Tech Stack

- Python 3.10+
- Libraries: `requests`, `beautifulsoup4`, `whois`, `shodan`, `nltk`, `spacy`, `openai`
- Optional GUI: `streamlit`
- Optional PDF: `reportlab`
- Optional local LLM: `llama-cpp-python`

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/reconai.git
cd reconai
pip install -r requirements.txt

ReconAI/
├── reconai.py                    # Main entry point
├── requirements.txt              # Python dependencies
├── README.md                     # Project README
├── .env                          # API keys (ignored by git)
├── /modules                      # Core recon modules
│   ├── whois_lookup.py
│   ├── subdomain_enum.py
│   ├── social_scraper.py
│   ├── shodan_lookup.py
│   ├── ai_analyzer.py
├── /utils                        # Helper functions
│   ├── report_generator.py
│   ├── config_loader.py
│   └── logger.py
├── /reports                      # Generated reports
│   ├── targetname_report.pdf
├── /dashboard                    # Streamlit UI
│   ├── app.py
│   └── components.py
├── /models                       # Optional: LLM/NER models
│   └── spacy_ner_model/
└── /docs                         # Architecture diagrams, research notes
    ├── recon_flowchart.png
    └── module_notes.md
