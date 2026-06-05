# ai-from-scratch

Building AI and deep learning models from scratch in PyTorch.

This repo is my hands-on journey of implementing everything from the ground up — no shortcuts, no black-box libraries. The goal is to deeply understand how modern AI systems work by building them myself, applied to real-world problems in finance and healthcare.

---

## projects

### 01 — credit risk prediction
**Scenario:** a bank needs to decide who to give a loan to. Wrong decisions cost real money — missing a defaulter is far more expensive than rejecting a good customer.  
**Built with:** logistic regression from scratch in numpy  
**Key questions:** why does linear regression fail for classification? how do you evaluate a model when errors have unequal costs?

---

### 02 — customer churn prediction
**Scenario:** a telecom company loses thousands of dollars per churned customer. They want to identify who is about to leave before they do so retention teams can intervene.  
**Built with:** neural network + backpropagation from scratch in numpy  
**Key questions:** how does learning actually happen mathematically? what happens when logistic regression can't capture complex feature interactions?

---

### 03 — skin lesion classification
**Scenario:** a model that looks at dermoscopy images and flags potentially malignant lesions. Misclassifying a malignant lesion as benign could cost someone their life.  
**Built with:** CNN in PyTorch trained on medical image data  
**Key questions:** how does spatial structure change modeling? why are convolutions more efficient than fully connected layers for images?

---

### 04 — toxic comment detection
**Scenario:** a platform needs to automatically flag harmful comments before human moderators review them. Context is everything — the same word means different things in different sentences.  
**Built with:** transformer + self-attention from scratch in PyTorch  
**Key questions:** why did attention replace RNNs? how does a model understand relationships between words across a full sentence?

---

### 05 — medical note generation
**Scenario:** doctors spend enormous time writing clinical notes after patient visits. A model trained on medical text learns the structure and terminology of clinical documentation and helps complete partial notes.  
**Built with:** character-level language model using the transformer from project 04  
**Key questions:** how does a model learn to generate rather than classify? what happens when the training domain is narrow and specialized?

---

### 06 — financial sentiment analysis and report summarization
**Scenario:** a hedge fund analyst reads hundreds of earnings reports and SEC filings daily. A fine-tuned model classifies sentiment (bullish, bearish, neutral) and summarizes long reports into key takeaways.  
**Built with:** GPT-2 fine-tuned on financial text using LoRA  
**Key questions:** how does transfer learning work? why is fine-tuning more efficient than training from scratch?

---

### 07 — legal knowledge base assistant
**Scenario:** a law firm has thousands of case files and legal precedents stored internally. Junior lawyers waste hours searching for relevant cases. A RAG system lets them ask natural language questions and get back relevant document excerpts with citations.  
**Built with:** RAG system with vector database and embedding model  
**Key questions:** how does semantic search work? when is RAG better than fine-tuning?

---

### 08 — algorithmic trading agent
**Scenario:** an agent that learns to buy, hold, or sell a portfolio of assets to maximize risk-adjusted returns. No labeled data — only the reward signal of profit and loss.  
**Built with:** deep RL agent (PPO) trained on historical market data  
**Key questions:** how does an agent learn from interaction rather than data? how do you handle delayed rewards and a non-stationary environment?

---

## the thread connecting all 8

Each project answers a question the previous one left open:

- logistic regression can't learn complex patterns → add layers (02)
- flat layers ignore structure → use convolutions (03)
- convolutions don't handle sequences → use attention (04)
- classification isn't generation → build a generative model (05)
- training from scratch is expensive → fine-tune what exists (06)
- fine-tuning can't handle new knowledge → retrieve it instead (07)
- supervised learning needs labels → learn from interaction (08)

This is not 8 random projects. It is the history of deep learning told through code, applied to real problems.

---

## where this is going

After these 8 projects the goal is to specialize in **financial AI and AI agents** — building systems that can autonomously analyze markets, retrieve relevant information, and make decisions. The intersection of finance domain knowledge and AI engineering is where I want to operate.

---

## stack
Python · PyTorch · numpy · HuggingFace · LangChain

---

## progress log
| project | status | date |
|---------|--------|------|
| 01 credit risk prediction | not started | |
| 02 customer churn prediction | not started | |
| 03 skin lesion classification | not started | |
| 04 toxic comment detection | not started | |
| 05 medical note generation | not started | |
| 06 financial sentiment analysis | not started | |
| 07 legal knowledge base assistant | not started | |
| 08 algorithmic trading agent | not started | |
