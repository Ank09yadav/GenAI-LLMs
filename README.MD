# Generative AI & Large Language Models (LLMs) — Comprehensive Guide & Interview Repository

Welcome to the definitive, production-grade technical interview and conceptual reference guide for **Generative AI and Large Language Models (LLMs)**.

This repository covers **90 curated questions** spanning fundamental theory, neural architectures, tokenization, distributed training, decoding strategies, parameter-efficient adaptation, evaluation methodologies, safety guardrails, production system design, and real-world troubleshooting.

All content is structured into **11 categorized folders**, with **one dedicated markdown file per question** formatted with mathematical rigor, architectural ASCII diagrams, comparative analysis tables, and senior/staff-level interview takeaways.

---

## 📚 Master Table of Contents

### [01. GenAI Fundamentals](01_genai_fundamentals/) (Questions 01 – 07)
Foundations of generative vs discriminative systems, emergent capabilities, and modern LLM architecture.
- **[01.md](01_genai_fundamentals/01.md)** — What is Generative AI?
- **[02.md](01_genai_fundamentals/02.md)** — How is Generative AI different from traditional Machine Learning?
- **[03.md](01_genai_fundamentals/03.md)** — What is an LLM?
- **[04.md](01_genai_fundamentals/04.md)** — What are the major components of a modern LLM system?
- **[05.md](01_genai_fundamentals/05.md)** — What types of tasks can LLMs perform?
- **[06.md](01_genai_fundamentals/06.md)** — What are the limitations of LLMs?
- **[07.md](01_genai_fundamentals/07.md)** — What is the difference between a foundation model and a task-specific model?

---

### [02. Transformers Architecture & Attention](02_transformers/) (Questions 08 – 17)
The mathematics of self-attention, multi-head subspaces, positional encodings, and scaling bottlenecks.
- **[08.md](02_transformers/08.md)** — Why were Transformers introduced?
- **[09.md](02_transformers/09.md)** — What problem do Transformers solve compared with RNNs?
- **[10.md](02_transformers/10.md)** — What is the Transformer architecture?
- **[11.md](02_transformers/11.md)** — What are Query, Key, and Value?
- **[12.md](02_transformers/12.md)** — How does self-attention work?
- **[13.md](02_transformers/13.md)** — What is multi-head attention?
- **[14.md](02_transformers/14.md)** — What is positional encoding?
- **[15.md](02_transformers/15.md)** — What is the difference between encoder-only, decoder-only, and encoder-decoder Transformers?
- **[16.md](02_transformers/16.md)** — Why are modern LLMs predominantly decoder-based?
- **[17.md](02_transformers/17.md)** — What is the computational challenge of self-attention?

---

### [03. Tokenization & Embeddings](03_tokenization_and_embeddings/) (Questions 18 – 25)
Subword segmentations, Byte-Pair Encoding (BPE), SentencePiece, vector geometry, and context inflation drivers.
- **[18.md](03_tokenization_and_embeddings/18.md)** — What is tokenization?
- **[19.md](03_tokenization_and_embeddings/19.md)** — Why don't LLMs directly process raw text?
- **[20.md](03_tokenization_and_embeddings/20.md)** — What are subword tokenization methods?
- **[21.md](03_tokenization_and_embeddings/21.md)** — What are BPE and SentencePiece at a high level?
- **[22.md](03_tokenization_and_embeddings/22.md)** — What is a token and how is it different from a word?
- **[23.md](03_tokenization_and_embeddings/23.md)** — What are embeddings?
- **[24.md](03_tokenization_and_embeddings/24.md)** — How are text embeddings different from token representations inside an LLM?
- **[25.md](03_tokenization_and_embeddings/25.md)** — What factors affect token count and context usage?

---

### [04. LLM Training Lifecycle](04_llm_training/) (Questions 26 – 34)
The end-to-end training pipeline from pretraining and scaling laws to SFT, instruction tuning, RLHF, and DPO.
- **[26.md](04_llm_training/26.md)** — How is an LLM trained?
- **[27.md](04_llm_training/27.md)** — What is pretraining?
- **[28.md](04_llm_training/28.md)** — What is next-token prediction?
- **[29.md](04_llm_training/29.md)** — What is the training objective of a causal language model?
- **[30.md](04_llm_training/30.md)** — What are training data, parameters, and compute in LLM training?
- **[31.md](04_llm_training/31.md)** — What is supervised fine-tuning?
- **[32.md](04_llm_training/32.md)** — What is instruction tuning?
- **[33.md](04_llm_training/33.md)** — What is RLHF?
- **[34.md](04_llm_training/34.md)** — What is DPO and how does it differ conceptually from RLHF?

---

### [05. Prompt Engineering & In-Context Learning](05_prompt_engineering/) (Questions 35 – 42)
In-context conditioning, Chain-of-Thought, ChatML roles, constrained grammars, and production prompt architecture.
- **[35.md](05_prompt_engineering/35.md)** — What is prompt engineering?
- **[36.md](05_prompt_engineering/36.md)** — What makes a good prompt?
- **[37.md](05_prompt_engineering/37.md)** — Zero-shot vs few-shot prompting?
- **[38.md](05_prompt_engineering/38.md)** — What is chain-of-thought prompting?
- **[39.md](05_prompt_engineering/39.md)** — What are system, user, and assistant messages?
- **[40.md](05_prompt_engineering/40.md)** — What is structured output and why is it useful?
- **[41.md](05_prompt_engineering/41.md)** — What is prompt injection?
- **[42.md](05_prompt_engineering/42.md)** — How would you design a prompt for a production application?

---

### [06. LLM Inference & Decoding Strategies](06_llm_inference/) (Questions 43 – 50)
Prefill vs decode phases, logit transformations, temperature, top-k/top-p sampling, greedy decoding, and KV cache sizing.
- **[43.md](06_llm_inference/43.md)** — What happens when an LLM generates a response?
- **[44.md](06_llm_inference/44.md)** — What are logits?
- **[45.md](06_llm_inference/45.md)** — How are logits converted into token probabilities?
- **[46.md](06_llm_inference/46.md)** — What is temperature?
- **[47.md](06_llm_inference/47.md)** — What are top-k and top-p sampling?
- **[48.md](06_llm_inference/48.md)** — Temperature vs top-p?
- **[49.md](06_llm_inference/49.md)** — What is greedy decoding?
- **[50.md](06_llm_inference/50.md)** — How do context length and KV cache affect inference?

---

### [07. Fine-Tuning, PEFT, LoRA & Quantization](07_fine_tuning_and_adaptation/) (Questions 51 – 58)
Domain adaptation trade-offs, Low-Rank Adaptation (LoRA), QLoRA, post-training quantization, and catastrophic forgetting.
- **[51.md](07_fine_tuning_and_adaptation/51.md)** — When should you fine-tune an LLM instead of using prompting?
- **[52.md](07_fine_tuning_and_adaptation/52.md)** — Fine-tuning vs RAG — when would you use each?
- **[53.md](07_fine_tuning_and_adaptation/53.md)** — What is parameter-efficient fine-tuning?
- **[54.md](07_fine_tuning_and_adaptation/54.md)** — What is LoRA?
- **[55.md](07_fine_tuning_and_adaptation/55.md)** — What is QLoRA?
- **[56.md](07_fine_tuning_and_adaptation/56.md)** — What is quantization?
- **[57.md](07_fine_tuning_and_adaptation/57.md)** — What are the tradeoffs of fine-tuning an LLM?
- **[58.md](07_fine_tuning_and_adaptation/58.md)** — What problems can occur during fine-tuning?

---

### [08. LLM Evaluation, Benchmarks & Metrics](08_llm_evaluation/) (Questions 59 – 66)
Evaluation in open-ended generative space, cross-entropy, perplexity, human vs automated benchmarks, LLM judges, and the RAG triad.
- **[59.md](08_llm_evaluation/59.md)** — Why is evaluating LLMs difficult?
- **[60.md](08_llm_evaluation/60.md)** — What is the difference between traditional ML evaluation and LLM evaluation?
- **[61.md](08_llm_evaluation/61.md)** — What are perplexity and cross-entropy?
- **[62.md](08_llm_evaluation/62.md)** — What are human evaluation and automated evaluation?
- **[63.md](08_llm_evaluation/63.md)** — What is an LLM-as-a-judge?
- **[64.md](08_llm_evaluation/64.md)** — How would you evaluate factuality?
- **[65.md](08_llm_evaluation/65.md)** — How would you evaluate an LLM application in production?
- **[66.md](08_llm_evaluation/66.md)** — What metrics would you track for an LLM application?

---

### [09. Hallucination, Safety & Reliability](09_hallucination_safety_and_reliability/) (Questions 67 – 74)
Root causes of confabulation, grounding verification, direct/indirect prompt injection, jailbreaking vectors, and defense-in-depth guardrails.
- **[67.md](09_hallucination_safety_and_reliability/67.md)** — What is an LLM hallucination?
- **[68.md](09_hallucination_safety_and_reliability/68.md)** — Why do LLMs hallucinate?
- **[69.md](09_hallucination_safety_and_reliability/69.md)** — How can hallucinations be reduced?
- **[70.md](09_hallucination_safety_and_reliability/70.md)** — What is grounding?
- **[71.md](09_hallucination_safety_and_reliability/71.md)** — What is prompt injection? (in safety/security context)
- **[72.md](09_hallucination_safety_and_reliability/72.md)** — What is jailbreak behavior?
- **[73.md](09_hallucination_safety_and_reliability/73.md)** — How would you build guardrails around an LLM application?
- **[74.md](09_hallucination_safety_and_reliability/74.md)** — How would you handle sensitive or untrusted input?

---

### [10. LLM Application Architecture & Production Engineering](10_llm_application_architecture/) (Questions 75 – 82)
Enterprise gateway architecture, request lifecycle, Server-Sent Events (SSE) streaming, latency and cost engineering, resilience, and distributed telemetry.
- **[75.md](10_llm_application_architecture/75.md)** — What does a typical production LLM application look like?
- **[76.md](10_llm_application_architecture/76.md)** — What happens between a user's request and the final LLM response?
- **[77.md](10_llm_application_architecture/77.md)** — How would you build an LLM API?
- **[78.md](10_llm_application_architecture/78.md)** — What is streaming generation?
- **[79.md](10_llm_application_architecture/79.md)** — How would you reduce LLM latency?
- **[80.md](10_llm_application_architecture/80.md)** — How would you control LLM API costs?
- **[81.md](10_llm_application_architecture/81.md)** — How would you handle rate limits and failures?
- **[82.md](10_llm_application_architecture/82.md)** — How would you monitor an LLM application?

---

### [11. Practical Scenarios & System Design](11_practical_scenarios_and_system_design/) (Questions 83 – 90)
Production incident triage, prompt regression debugging, financial optimization, model selection, 1M DAU system design, and complete real-world case study.
- **[83.md](11_practical_scenarios_and_system_design/83.md)** — Your LLM gives correct answers for some questions but hallucinates on others. How would you debug it?
- **[84.md](11_practical_scenarios_and_system_design/84.md)** — Your prompts work well in testing but fail in production. What would you investigate?
- **[85.md](11_practical_scenarios_and_system_design/85.md)** — Your LLM application is too expensive. How would you reduce cost?
- **[86.md](11_practical_scenarios_and_system_design/86.md)** — Your application has high latency. How would you optimize it?
- **[87.md](11_practical_scenarios_and_system_design/87.md)** — How would you choose between prompting, RAG, and fine-tuning?
- **[88.md](11_practical_scenarios_and_system_design/88.md)** — How would you choose an LLM for a production application?
- **[89.md](11_practical_scenarios_and_system_design/89.md)** — How would you design an LLM application for 1 million users?
- **[90.md](11_practical_scenarios_and_system_design/90.md)** — Walk through the architecture of an LLM project you built.

---

## 🎯 How to Use This Repository

1. **For Interview Preparation:** Review the `Key Point` and `Interview Answer` sections at the end of each file for concise, high-impact phrasing tailored for technical interview discussions.
2. **For Architecture & System Design:** Study modules `02`, `06`, `07`, `10`, and `11` for latency formulas, GPU memory budgeting, distributed serving, and multi-tier production system architectures.
3. **For Hands-on Implementation:** Utilize the production FastAPI endpoints, structured JSON Pydantic patterns, and error handling implementations provided throughout the files.