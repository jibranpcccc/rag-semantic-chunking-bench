# RAGInspect RAG Chunking & Embedding Retrieval Benchmarks

Empirical retrieval accuracy (NDCG@10, MRR@10) across chunking strategies: Fixed-Size, Recursive, Semantic Similarity, and ColPali.

⚡ **Test Chunking Strategies:** [https://raginspect.pages.dev/](https://raginspect.pages.dev/)

## 1. Retrieval Accuracy on Financial Documents (10-K Filings)

| Chunking Strategy | Chunk Size / Param | NDCG@10 | Table Retrieval Accuracy | Ingestion Speed |
| :--- | :--- | :--- | :--- | :--- |
| ColPali Vision-Language | Native 448x448 Patch | 0.884 | 94.2% | 180 ms / page |
| Semantic Boundary (Cosine 0.8) | Dynamic 200-800 tok | 0.812 | 68.5% | 450 ms / page |
| Recursive Character Splitter | 512 tok (10% overlap) | 0.742 | 48.1% | 25 ms / page |
| Fixed Token Splitter | 500 tok (0 overlap) | 0.690 | 38.0% | 15 ms / page |

---
Maintained by [RAGInspect](https://raginspect.pages.dev/).

## 📚 In-Depth Technical Implementation Guides

| Target Engineering Query | Production Reference & Guide URL |
| :--- | :--- |
| **Rag Semantic Chunking Benchmark** | [https://raginspect.pages.dev/semantic-chunking-vs-fixed-size-rag-benchmarks/](https://raginspect.pages.dev/semantic-chunking-vs-fixed-size-rag-benchmarks/) |
| **Hybrid Search Bm25 Dense Vector Accuracy** | [https://raginspect.pages.dev/hybrid-search-bm25-vs-dense-vector-accuracy/](https://raginspect.pages.dev/hybrid-search-bm25-vs-dense-vector-accuracy/) |
| **Recursive Character Text Splitter Vs Semantic Chunking** | [https://raginspect.pages.dev/recursive-vs-semantic-chunking/](https://raginspect.pages.dev/recursive-vs-semantic-chunking/) |
| **Bm25 K1 B Parameter Tuning Rag** | [https://raginspect.pages.dev/bm25-k1-b-hyperparameter-tuning/](https://raginspect.pages.dev/bm25-k1-b-hyperparameter-tuning/) |

