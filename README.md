# From Predictive to Generative AI: Workshop Materials

## 🎯 Workshop Overview

This 60-minute workshop demonstrates the paradigm shift from traditional Predictive AI to modern Generative AI through hands-on coding and practical examples.

**Target Audience**: Beginner to Advanced(mixed coding experience)  
**Duration**: 60 minutes  
**Platform**: Google Colab and Visual Studio Code  


## 📁 File Structure

```
Hackfest-Machakos/
├── 01_Predictive_AI_Titanic_Classification.ipynb    # Traditional ML demo
├── 02_Generative_AI_Working_Demo.ipynb              # Generative AI demo with chat
├── Workshop_Presenter_Notes.md                      # Detailed presenter guide
├── requirements.txt                                  # Python dependencies
└── README.md                                         # This file
```

## 📚 Workshop Materials

### 1. Core Notebooks
- **`01_Predictive_AI_Titanic_Classification.ipynb`**: Traditional ML pipeline using Logistic Regression
- **`02_Generative_AI_Working_Demo.ipynb`**: Generative AI with Gemini/Ollama + interactive chat

### 2. Presenter Resources
- **`Workshop_Presenter_Notes.md`**: Detailed 60-minute timeline with talking points and engagement strategies
- **`requirements.txt`**: All required Python packages

## 🚀 Quick Start Guide

### For Presenters:
1. Review the presenter notes thoroughly
2. Test both notebooks in Google Colab
3. Obtain a free Gemini API key from [Google AI Studio](https://makersuite.google.com/)
4. Practice the key analogies and transitions

### For Participants:
1. Open Google Colab in your browser
2. Upload the notebook files or access via shared links
3. Follow along with the live demonstration
4. Experiment with prompt modifications

## 🎓 Learning Objectives

By the end of this workshop, participants will:

- **Understand** the fundamental differences between Predictive and Generative AI
- **Experience** the traditional ML pipeline: Load → Clean → Train → Predict
- **Master** basic prompt engineering techniques
- **Compare** cloud-based vs local AI deployment options
- **Apply** appropriate AI approaches to hackathon projects

## 🔧 Technical Requirements

### Prerequisites:
- **Python 3.8+** (for local development)
- **Web browser** with internet connection
- **Google account** (for Colab access)
- **Basic Python familiarity** (helpful but not required)

### Required Packages:
Install all dependencies with:
```bash
pip install -r requirements.txt
```

**Core Libraries:**
- `pandas>=2.0.0` - Data manipulation
- `numpy>=1.24.0` - Numerical operations
- `scikit-learn>=1.3.0` - Machine learning
- `matplotlib>=3.7.0` - Plotting
- `seaborn>=0.12.0` - Statistical visualization
- `google-generativeai>=0.8.0` - Gemini AI integration
- `requests>=2.31.0` - HTTP requests for Ollama

### Optional Enhancements:
- **Gemini API key** (free from [Google AI Studio](https://makersuite.google.com/))
- **Local Ollama installation** for privacy-focused AI ([ollama.ai](https://ollama.ai))

## 📖 Workshop Structure

### Phase 1: The "Predict" World (0-10 min)
- Traditional ML demonstration with Titanic dataset
- Four-step pipeline: Load → Clean → Train → Predict
- Key limitation: Can only output known categories

### Phase 2: The "Generate" World (10-25 min)
- Introduction to Large Language Models
- Prompt engineering as the new programming paradigm
- Cloud vs local AI deployment strategies

### Phase 3: Hands-On Showdown (25-45 min)
- Live coding with Gemini and Ollama
- Student experimentation with prompt modifications
- Results sharing and discussion

### Phase 4: Hackfest Strategy (45-60 min)
- Choosing the right AI approach for projects
- Ethical considerations and responsible AI use
- Practical next steps and resources

## 🎯 Key Concepts Covered

### Traditional ML Concepts:
- Supervised learning and classification
- Data preprocessing and feature engineering
- Model training and evaluation
- Prediction accuracy and limitations

### Generative AI Concepts:
- Large Language Models (LLMs)
- Prompt engineering techniques
- Role-based AI interactions
- Multimodal AI capabilities

### Practical Skills:
- Google Colab usage
- API integration (Gemini)
- Local AI setup (Ollama)
- Prompt optimization strategies

## 🛠️ Setup Instructions

### Option 1: Google Colab (Recommended)
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Upload the `.ipynb` files or open from GitHub
3. Run cells sequentially - packages install automatically
4. Add Gemini API key when prompted

### Option 2: Local Development
1. **Clone/Download** this repository
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Start Jupyter**:
   ```bash
   jupyter notebook
   ```
4. **Open notebooks** and run cells sequentially

### API Setup (Optional but Recommended)

#### Gemini API (Cloud AI):
1. Visit [Google AI Studio](https://makersuite.google.com/)
2. Create free account and generate API key
3. In notebook, replace `YOUR_API_KEY_HERE` with your key
4. **Security**: Never commit API keys to version control!

#### Ollama (Local AI):
1. Install from [ollama.ai](https://ollama.ai)
2. Download model: `ollama pull llama3`
3. Start server: `ollama serve`
4. Notebook will auto-detect local server

## 🎨 Customization Options

### Adapt for Different Audiences:
- **Beginner Coders**: Focus more on concepts and analogies
- **Advanced Developers**: Add technical deep-dives and optimization
- **Non-Technical**: Emphasize practical applications and prompt engineering

### Extend the Workshop:
- Add computer vision examples with Gemini's multimodal capabilities
- Include fine-tuning demonstrations
- Explore different AI model comparisons
- Add ethical AI discussion sessions

## 📊 Assessment & Outcomes

### Immediate Success Indicators:
- Students can explain Predictive vs Generative AI differences
- 50%+ successfully run at least one notebook
- Active participation in prompt engineering exercises
- Questions about practical applications

### Hackathon Impact Metrics:
- Teams incorporate AI thoughtfully into projects
- Evidence of prompt engineering in presentations
- Appropriate AI approach selection for problems
- Responsible AI usage considerations

## 🔗 Additional Resources

### Free AI APIs:
- [Google AI Studio](https://makersuite.google.com/) - Gemini API
- [OpenAI Platform](https://platform.openai.com/) - GPT models
- [Hugging Face](https://huggingface.co/) - Open source models

### Local AI Tools:
- [Ollama](https://ollama.ai/) - Local LLM runner
- [LM Studio](https://lmstudio.ai/) - GUI for local models
- [GPT4All](https://gpt4all.io/) - Privacy-focused AI

### Learning Materials:
- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [Fast.ai Practical Deep Learning](https://course.fast.ai/)
- [Coursera AI for Everyone](https://www.coursera.org/learn/ai-for-everyone)

## 🤝 Contributing

This workshop is designed to be adapted and improved. Feel free to:
- Modify notebooks for your specific audience
- Add new examples and use cases
- Translate materials to other languages
- Share improvements and feedback

## 📄 License

These materials are provided for educational use. Please respect API terms of service and model usage policies when using external AI services.

## 🎓 Workshop Learning Path

### Phase 1: Traditional ML (0-15 min)
- Load and explore Titanic dataset
- Build Logistic Regression model
- Understand limitations: only predicts 0/1

### Phase 2: Generative AI (15-45 min)
- Compare AI approaches: Gemini vs Ollama vs Rules
- Learn prompt engineering techniques
- Experience natural language predictions

### Phase 3: Interactive AI Chat (45-60 min)
- Ask AI questions about the data
- Get insights and explanations
- Understand AI as analysis partner

## 🆘 Troubleshooting

### Common Issues:
- **Package errors**: Run `pip install -r requirements.txt`
- **Colab crashes**: Restart runtime and run cells again
- **API key errors**: Verify key is correct and has quota
- **Ollama connection fails**: Expected in Colab (local only)
- **Slow responses**: Try simpler prompts or different models

### Getting Help:
- Check notebook comments for detailed explanations
- Review `Workshop_Presenter_Notes.md` for context
- Test in fresh environment before presenting

## 📊 Success Metrics

### Immediate Indicators:
- Students explain Predictive vs Generative AI differences
- 70%+ successfully run at least one notebook
- Active participation in chat experiments
- Questions about practical applications

### Hackathon Impact:
- Teams incorporate AI thoughtfully into projects
- Evidence of prompt engineering in presentations
- Appropriate AI approach selection for problems

## 🤝 Contributing & Feedback

This workshop is designed to be adapted and improved:
- Modify notebooks for your specific audience
- Add new examples and use cases
- Translate materials to other languages
- Share improvements and feedback

## 📄 License

These materials are provided for educational use. Please respect API terms of service and model usage policies.

**Ready to explore the future of AI? Let's dive in! 🚀**

*Last updated: 21st, October 2025*