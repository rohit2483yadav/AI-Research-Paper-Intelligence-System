
# AI Research Paper Intelligence System

AI Research Paper Intelligence System is an NLP-based application that helps users search, analyze, and understand research papers using semantic search, transformer models, vector databases, and Large Language Models (LLMs).

The system retrieves the most relevant research papers for a given query, generates concise summaries, extracts important keywords and research entities, and visualizes the similarity between retrieved papers.

##  Features

###  Semantic Research Paper Search
- Search research papers using natural language queries.
- Uses Sentence Transformers for semantic embeddings.
- Retrieves the most relevant papers using FAISS vector search.

---

###  AI-powered Summarization
- Generates concise summaries of research paper abstracts.
- Built using Facebook's BART Large CNN summarization model.

---

###  Keyword Extraction
Automatically extracts important keywords and phrases from each research paper using KeyBERT.

Example:

- Deep Learning
- Medical Imaging
- CNN
- Image Reconstruction

---

###  LLM-based Research Entity Extraction

Uses Google Gemini to intelligently extract structured research information.

Extracted entities include:

- Models
- Datasets
- Methods
- Frameworks
- Metrics
- Optimizers

Example:

```json
{
  "Models": ["CNN", "ResNet"],
  "Datasets": ["ImageNet"],
  "Methods": ["Transfer Learning"],
  "Frameworks": ["PyTorch"],
  "Metrics": ["Accuracy"],
  "Optimizers": ["Adam"]
}
```

---

###  Similarity Heatmap

Visualizes how similar the retrieved research papers are to each other using cosine similarity.

This helps users quickly understand:

- Similar research topics
- Closely related papers
- Paper clusters

---



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
