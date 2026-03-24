# Workshop Presenter Notes: From Predictive to Generative AI

## UbuCon Africa 2026 Format (1 hr 45 min)

**Duration**: 105 minutes
**Audience**: Intermediate (mixed coding experience)
**Materials**: 3 notebooks + 22-slide Beamer presentation
**Primary AI**: Ollama (local) | **Secondary**: Gemini (cloud)

---

### Pre-Session Checklist

- [ ] Test all 3 notebooks in fresh Colab environment
- [ ] Verify Ollama is running locally with llama3 model
- [ ] Verify Gemini API key works (backup)
- [ ] Compile presentation: `xelatex presentation.tex`
- [ ] Have presentation PDF open and ready
- [ ] Pre-load notebook outputs in case of technical issues
- [ ] Test screen sharing, audio, and projector
- [ ] Share notebook links / GitHub repo in chat

---

### Detailed Timeline

#### Phase 1: Opening & Presentation (0-15 min)

| Time | Action | Notes |
|------|--------|-------|
| 0-2 min | **Opening hook** | "Who has used ChatGPT? Now, who understands HOW it works differently from traditional programming?" |
| 2-5 min | **Slides 1-6**: AI landscape | Two Worlds of AI — Predictive vs Generative comparison. Use the detective vs conversation analogy. |
| 5-10 min | **Slides 7-10**: Key concepts | Prompt engineering as the new programming. Recipe vs magic spell analogy. |
| 10-13 min | **Slides 11-14**: Decision framework | When to use Predictive vs Generative. Tool selection analogy. |
| 13-15 min | **Transition to Demo 1** | "Let's see the traditional approach in action. Open your notebooks!" |

**Energy**: High. Set expectations. Get hands raised.

#### Phase 2: Live Demo 1 — Predictive AI (15-35 min)

**Notebook**: `01_Predictive_AI_Titanic.ipynb`

| Time | Action | Notes |
|------|--------|-------|
| 15-18 min | **Setup & data loading** | Run first cells. "We're detectives studying 1912 passenger records." |
| 18-22 min | **3-panel visualization** | Explore survival by class, gender, age. Let the data tell its story. |
| 22-26 min | **Data cleaning & training** | Show the 4-step pipeline: Load > Clean > Train > Predict. Emphasize rigidity. |
| 26-30 min | **Feature importance + confusion matrix** | "The model learned that gender and class matter most." |
| 30-33 min | **New passenger predictions** | Predict for custom passengers. Show it only outputs 0 or 1. |
| 33-35 min | **Limitation framing** | **KEY MOMENT**: "This model can ONLY say survived/died. It cannot explain WHY. It cannot create anything new. It cannot speak Kiswahili." |

**Transition**: "What if we could just ASK the AI in plain English... or Kiswahili?"

#### Phase 3: Live Demo 2 — Generative AI (35-65 min)

**Notebook**: `02_Generative_AI_Demo.ipynb`

| Time | Action | Notes |
|------|--------|-------|
| 35-38 min | **Setup** | Install packages, configure Ollama/Gemini. |
| 38-42 min | **Prompt engineering** | Show anatomy of a good prompt. Role + context + task + constraints. |
| 42-48 min | **Ollama demo** | Local AI interaction. "This runs entirely on YOUR machine. No data leaves." Privacy angle for Ubuntu/FOSS audience. |
| 48-52 min | **Gemini demo** | Cloud AI comparison. Faster, more capable, but data goes to Google. |
| 52-57 min | **AI Showdown** | Same Titanic question to both models. Compare responses side-by-side. |
| 57-62 min | **Interactive chat** | Use `chat()` function. Let audience suggest questions. |
| 62-65 min | **Prompt Playground** | Quick demo of the 3 experiments. Tease what participants will try themselves. |

**Key talking points**:
- "We just solved the same problem by having a conversation. No training data needed."
- "Ollama = home cooking (private, customizable). Gemini = restaurant delivery (fast, convenient)."
- "The prompt IS your program."

#### Phase 4: Live Demo 3 — Kiswahili AI (65-80 min)

**Notebook**: `03_Generative_AI_Kiswahili.ipynb`

| Time | Action | Notes |
|------|--------|-------|
| 65-68 min | **Motivation** | "AI shouldn't only work in English. Let's make it speak Kiswahili." UbuCon Africa context — AI for African languages. |
| 68-72 min | **Setup & system prompt** | Show `KISWAHILI_SYSTEM` prompt. "One instruction changes the entire AI personality." |
| 72-75 min | **Data in Kiswahili** | Run `pata_takwimu()`. Show Kiswahili variable names and output. |
| 75-78 min | **Chat in Kiswahili** | Use `zungumza()` function. Ask questions in Kiswahili, get Kiswahili answers. |
| 78-80 min | **Prompt experiments** | Show how changing the system prompt changes language, tone, expertise. |

**Key talking points**:
- "This is the same AI, same model — just a different system prompt."
- "Imagine building apps that serve communities in their own language."
- "The fallback chain (Data > Ollama > Gemini > Akiba) ensures something always works."

#### Phase 5: Hands-On & Closing (80-105 min)

| Time | Action | Notes |
|------|--------|-------|
| 80-85 min | **Setup help** | Help participants get notebooks running. Troubleshoot issues. |
| 85-95 min | **Free experimentation** | Participants modify prompts, try different questions, break things. Walk around and help. |
| 95-100 min | **Show and tell** | Volunteers share interesting results. Highlight creative prompt engineering. |
| 100-103 min | **Decision framework recap** | When to use Predictive vs Generative. Ethical considerations. |
| 103-105 min | **Closing** | Share resources, GitHub link, contact info. "You now have tools that were science fiction 5 years ago." |

---

### Key Analogies

| Analogy | Predictive AI | Generative AI |
|---------|---------------|---------------|
| **Detective vs Consultant** | Studies past cases to predict | Consults an expert who explains |
| **Recipe vs Magic Spell** | Exact steps, predictable results | Right words create powerful results |
| **Calculator vs Assistant** | Precise but limited | Intelligent and creative |
| **Home Cooking vs Delivery** | Ollama: private, customizable | Gemini: fast, convenient |

### Audience Engagement

**For coders**: Show code, discuss API details, challenge them to optimize prompts.
**For non-coders**: Focus on analogies, emphasize prompt engineering as "programming with words."
**For the Ubuntu/FOSS crowd**: Emphasize Ollama's local-first, privacy-respecting approach. Open source models.

### Common Questions

**"Is Generative AI always better?"**
No. Need millisecond predictions on structured data? Use traditional ML. Need creative explanations or natural language? Use Generative AI. The future is hybrid.

**"Can I use this for free?"**
Ollama is completely free and local. Gemini has a generous free tier. Many open source models on Hugging Face.

**"Are AI models biased?"**
Yes. They learn from human data containing human biases. Always test with diverse inputs. Especially important for African language AI — models have less training data in Kiswahili.

**"How do I add other African languages?"**
Change the system prompt! Replace Kiswahili instructions with your target language. Works for any language the model was trained on.

### Backup Plans

| Problem | Solution |
|---------|----------|
| Ollama not working | Switch to Gemini as primary. Show Ollama setup steps for later. |
| Gemini API fails | Use Ollama only. Show pre-recorded Gemini outputs. |
| No internet | Use Ollama locally. Have pre-run notebooks with outputs saved. |
| Colab unavailable | Use local Jupyter. Provide pre-run HTML exports. |
| Participants can't follow | Pair experienced with beginners. Focus on prompt engineering on paper. |

---

## Hackfest Machakos 2025 Format (60 min)

Compact version using only 2 notebooks. No presentation slides, no Kiswahili notebook.

| Time | Phase | Content |
|------|-------|---------|
| 0-10 min | The "Predict" World | Hook with Titanic detective story. Run ML pipeline. Emphasize 0/1 limitation. |
| 10-25 min | The "Generate" World | Introduce LLMs, prompt engineering, cloud vs local. Conceptual transition. |
| 25-45 min | Hands-On Showdown | Live code Gemini/Ollama. Student experimentation. Results sharing. |
| 45-60 min | Hackfest Strategy | Choosing the right AI approach. Ethics. Resources. Inspiration for hackathon projects. |

Same analogies and engagement strategies apply — just compressed.

---

## Post-Workshop

- [ ] Share GitHub repo link: `https://github.com/Kevinobote/From-Predictive-to-Generative-AI`
- [ ] Share additional resources (AI APIs, learning materials)
- [ ] Collect feedback
- [ ] Note interesting participant discoveries for future workshops

---

**Remember**: Your enthusiasm is contagious. If you're excited about AI possibilities, your audience will be too. Focus on empowering them to build amazing things!
