
# AI Research Paper Intelligence System

AI Research Paper Analyzer is an NLP-based application that helps users search, analyze, and understand research papers using semantic search, transformer models, vector databases, and Large Language Models (LLMs).

The system retrieves the most relevant research papers for a given query, generates concise summaries, extracts important keywords and research entities, and visualizes the similarity between retrieved papers.

## Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| Dataset | ML-ArXiv Papers |
| Embedding Model | SentenceTransformer (all-MiniLM-L6-v2) |
| Vector Search | FAISS |
| Summarization | facebook/bart-large-cnn |
| Keyword Extraction | KeyBERT |
| LLM | Google Gemini 2.5 Flash |
| Visualization | Matplotlib |
| Similarity Metric | Cosine Similarity |


##  Project Architecture

User Query
│
▼
SentenceTransformer
(all-MiniLM-L6-v2)
│
▼
Query Embedding
│
▼
FAISS Vector Search
│
▼
Top-K Relevant Papers
│
├───────────────► BART
│ Summary
│
├───────────────► KeyBERT
│ Keywords
│
├───────────────► Gemini LLM
│ Research Entity Extraction
│
└───────────────► Similarity Heatmap




## Future Improvements

- Chat with Research Papers
- PDF Upload and Analysis
- Question Answering
- Paper Comparison
- Literature Review Generation
- Research Knowledge Graph
- Interactive Web Interface
