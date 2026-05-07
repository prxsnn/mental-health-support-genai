# mental-health-support-genai
- Built an end-to-end AI system integrating three large language models (Google Gemini,
  Meta Llama 3.3-70B, Qwen3-32B) for zero-shot mental health text classification and
  empathetic response generation

- Achieved 91.75% accuracy and 91.56% F1 score on binary mental health classification
  using Gemini with confidence-threshold prompting on a 400-sample balanced evaluation set

- Designed and implemented a Retrieval-Augmented Generation (RAG) pipeline using
  ChromaDB vector store and Google gemini-embedding-001 embeddings, indexing 515 text
  chunks from curated mental health knowledge documents

- Built a LangGraph agentic pipeline with conditional routing logic for dynamic
  query handling, automatically triggering RAG retrieval for high-severity or
  crisis-flagged inputs

- Conducted comparative evaluation of three LLMs (Gemini, Llama 3, Qwen3) across
  two prompt configurations, revealing that aggressive NLP preprocessing degrades
  zero-shot LLM classification by destroying contextual signals

- Performed exploratory data analysis on three real-world mental health datasets
  (27,977 + 232,074 + 1,259 records) using matplotlib, seaborn, and wordcloud,
  identifying a 3.3x word count disparity between crisis and non-crisis posts
