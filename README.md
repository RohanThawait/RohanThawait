# Hi, I'm Rohan Thawait 👋

M.Tech student at **NIT Karnataka (NITK Surathkal)** · Graduating June 2026  
I train large language models from scratch and build the systems around them.

---

## What I'm Working On

I spent the last several months going deep on LLM training — not using APIs, but actually training models on H100 hardware. Here's what that produced:

### 🧠 GRPO Reasoning Model — Qwen2.5-7B
Implemented the full reasoning training pipeline from the **DeepSeek-R1 paper**.  
SFT cold start on 27K math CoT examples → GRPO reinforcement learning with verifiable reward functions.  
The most interesting finding: diagnosed **reward saturation** from training curves — `frac_reward_zero_std` averaged 0.63, meaning 63% of batches produced near-zero gradient signal. Replicates the curriculum selection problem DeepSeek documented.

- 📊 MATH-500: **+3.6%** over instruct baseline (out-of-distribution generalization)  
- 🤗 [Model on HuggingFace](https://huggingface.co/thawait/qwen2.5-7b-math-reasoning-grpo)  
- 💻 [Code + benchmarks](https://github.com/RohanThawait/qwen2.5-7b-math-reasoning-grpo)  
- 🎤 [Live voice demo](https://huggingface.co/spaces/thawait/math-reasoning-voice-demo)

### 📐 Long-Context RoPE Scaling — Mistral-7B
Extended Mistral-7B context from 8K → 32K tokens using **YaRN RoPE scaling** + **LongLoRA** finetuning.  
Evaluated with needle-in-a-haystack tests across context lengths.

---

## Technical Stack

**LLM Training**  
`GRPO` `SFT` `Full Finetuning` `LoRA` `Reward Function Design` `BF16` `FlashAttention-2` `Gradient Checkpointing`

**Frameworks**  
`PyTorch` `HuggingFace TRL` `Transformers` `DeepSpeed` `lm-evaluation-harness` `Weights & Biases`

**Inference & Evaluation**  
`Speculative Decoding` `YaRN` `RoPE Scaling` `GSM8K` `MATH` `ARC benchmarks`

**Application Layer**  
`LangChain` `LangGraph` `FastAPI` `Streamlit` `RAG` `FAISS`

**Infrastructure**  
`H100 NVL` `CUDA` `Linux` `Docker` `Git` `HuggingFace Hub`

---

## Other Projects

| Project | What it does |
|---|---|
| [VoicePaper](https://github.com/RohanThawait) | Converts research papers into podcast audio — PyMuPDF → GPT-4 → ElevenLabs |
| [LawyerLens](https://github.com/RohanThawait) | RAG pipeline for legal document Q&A — FAISS + OpenAI embeddings |
| [FinancialAgent](https://github.com/RohanThawait) | LLM agent with conversational SQL, data viz, Plaid API integration |

---

## Background

- 🎓 M.Tech Computational and Data Science — **NIT Karnataka** (GATE CS 2024)
- 🎓 B.Tech Computer Science — SAGE University
- 💡 500+ LeetCode problems · Kaggle Contributor · Python Gold @ HackerRank

---

## Let's Talk

I'm open to **LLM Engineer**, **ML Engineer**, and **AI Engineer** roles — India and remote international.

📧 thawaitrohan@gmail.com  
🤗 [huggingface.co/thawait](https://huggingface.co/thawait)  
💼 [LinkedIn]([www.linkedin.com/in/rohan-thawait-7137081a5])]
