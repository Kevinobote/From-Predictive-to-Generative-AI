# From Predictive to Generative AI: A Hands-On Journey Through the AI Revolution

## Workshop Overview

A hands-on workshop demonstrating the paradigm shift from traditional Predictive AI to modern Generative AI through live coding, prompt engineering, and multilingual AI experiences.

**Presented at**: UbuCon Africa 2026 (1 hr 45 min)
**Technical Level**: Intermediate (mixed coding experience welcome)
**Platform**: Google Colab, VS Code, or local Jupyter

## File Structure

```
.
├── UbuCon-2026/                                      # UbuCon Africa 2026 materials
│   ├── 01_Predictive_AI_Titanic.ipynb                #   Traditional ML pipeline
│   ├── 02_Generative_AI_Demo.ipynb                   #   Generative AI with Ollama & Gemini
│   ├── 03_Generative_AI_Kiswahili.ipynb              #   AI in Kiswahili language
│   ├── presentation.tex                              #   Beamer slides (22 slides)
│   ├── presentation.pdf                              #   Compiled presentation
│   └── .gitignore                                    #   LaTeX auxiliary exclusions
├── Workshop_Presenter_Notes.md                       # Presenter guide
├── requirements.txt                                  # Python dependencies
└── README.md                                         # This file
```

## Workshop Structure

### Highlights
- **3 hands-on notebooks** — Predictive AI, Generative AI, and Kiswahili AI
- **22-slide Beamer presentation** for structured delivery
- **Ollama-first approach** — local AI as primary, Gemini as secondary
- **Multilingual AI** — full Kiswahili language experience
- **Extended hands-on time** — 45 minutes of participant experimentation

### Timeline

| Phase | Time | Content | Notebook |
|-------|------|---------|----------|
| Opening & Presentation | 0-15 min | AI landscape, key concepts | `presentation.pdf` |
| Live Demo 1: Predictive AI | 15-35 min | Titanic ML pipeline, limitations | `01_Predictive_AI_Titanic.ipynb` |
| Live Demo 2: Generative AI | 35-65 min | Prompt engineering, Ollama vs Gemini, AI Showdown | `02_Generative_AI_Demo.ipynb` |
| Live Demo 3: Kiswahili AI | 65-80 min | AI in African languages | `03_Generative_AI_Kiswahili.ipynb` |
| Hands-On & Closing | 80-105 min | Participant experimentation, Q&A | All notebooks |

### Notebooks

**01 - Predictive AI (Titanic Classification)**
- Load and explore Titanic dataset with 3-panel visualization
- Data cleaning and feature engineering
- Logistic Regression training with train/test split
- Feature importance + confusion matrix analysis
- New passenger predictions
- Critical framing: model can ONLY output 0 or 1

**02 - Generative AI Demo**
- Prompt engineering fundamentals (anatomy of a good prompt)
- Ollama local AI setup and interaction
- Gemini cloud AI integration
- AI Showdown: same question, different approaches compared
- Interactive chat function with Ollama > Gemini fallback
- Prompt Engineering Playground (3 experiments)

**03 - Generative AI in Kiswahili**
- Entirely in Kiswahili language
- `KISWAHILI_SYSTEM` prompt forces Kiswahili responses
- `pata_takwimu()` — dataset statistics with Kiswahili variable names
- `jibu_kutoka_data(swali)` — keyword-based Kiswahili data answers
- `zungumza(swali)` — unified chat (Data > Ollama > Gemini > Akiba fallback)
- Prompt engineering experiments in Kiswahili

### Presentation (22 Slides)
Built with LaTeX Beamer. Covers:
- Opening & AI landscape (2 slides)
- Two Worlds of AI comparison (2 slides)
- Generative AI concepts (3 slides)
- Kiswahili AI motivation (2 slides)
- Decision framework for choosing AI approaches (3 slides)
- Live demo transitions and closing (remaining slides)

Compile with: `xelatex presentation.tex` (requires `fontspec` package)

## Quick Start

### Prerequisites
- Python 3.8+
- Web browser with internet connection
- Google account (for Colab)

### Installation
```bash
git clone https://github.com/Kevinobote/From-Predictive-to-Generative-AI.git
cd From-Predictive-to-Generative-AI
pip install -r requirements.txt
```

### API Setup

**Ollama (Local AI — recommended):**
```bash
# Install from https://ollama.ai
ollama pull llama3.2:3b
ollama serve
```

**Gemini (Cloud AI — optional):**
1. Get free API key from [Google AI Studio](https://makersuite.google.com/)
2. Replace `YOUR_API_KEY_HERE` in notebooks
3. Never commit API keys to version control

### Running in Google Colab
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Upload `.ipynb` files or open from GitHub
3. Run cells sequentially — packages install automatically

## Learning Objectives

By the end of this workshop, participants will:
- Understand the fundamental differences between Predictive and Generative AI
- Experience the traditional ML pipeline: Load > Clean > Train > Predict
- Master basic prompt engineering techniques
- Compare cloud-based (Gemini) vs local (Ollama) AI deployment
- Experience AI in African languages (Kiswahili)
- Apply appropriate AI approaches to real projects

## Key Concepts

| Predictive AI | Generative AI |
|---------------|---------------|
| Supervised learning & classification | Large Language Models (LLMs) |
| Data preprocessing & feature engineering | Prompt engineering |
| Model training & evaluation | Role-based AI interactions |
| Outputs known categories only | Creates new, original content |
| Requires structured data | Works with natural language |

## Tech Stack

- **ML**: pandas, numpy, scikit-learn, matplotlib, seaborn
- **Generative AI**: Ollama (llama3), Google Gemini (gemini-2.0-flash)
- **Presentation**: LaTeX Beamer (xelatex)
- **Platform**: Google Colab, Jupyter Notebook

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Package errors | `pip install -r requirements.txt` |
| Colab crashes | Restart runtime, run cells again |
| API key errors | Verify key is correct and has quota |
| Ollama connection fails | Expected in Colab (local only) — install Ollama on your machine |
| Slow responses | Try simpler prompts or smaller models |
| LaTeX won't compile | Use `xelatex` not `pdflatex` (requires fontspec) |

## Resources

**AI APIs**: [Google AI Studio](https://makersuite.google.com/) | [Hugging Face](https://huggingface.co/) | [OpenAI](https://platform.openai.com/)
**Local AI**: [Ollama](https://ollama.ai/) | [LM Studio](https://lmstudio.ai/) | [GPT4All](https://gpt4all.io/)
**Learning**: [Prompt Engineering Guide](https://www.promptingguide.ai/) | [Fast.ai](https://course.fast.ai/) | [Coursera AI for Everyone](https://www.coursera.org/learn/ai-for-everyone)

## Contributing

This workshop is designed to be adapted. Feel free to:
- Modify notebooks for your audience
- Add new language versions (like the Kiswahili notebook)
- Translate materials
- Share improvements and feedback

## License

Educational use. Please respect API terms of service and model usage policies.

---

*Last updated: June 2025*
