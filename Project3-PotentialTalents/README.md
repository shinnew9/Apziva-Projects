# Project 3: 
LLM-Based Semantic Candidate Ranking

## Objective
- Enable semantic matching between job descriptions and candidate profiles
- Move beyond keyword-based search toward meaning-aware candidate ranking
- Design an efficient LLM-based pipeline for retrieval and ranking in recruitment scenarios

## Architecture
- **Data Input**
  - Job descriptions and candidate profile text
- **Text Representation**
  - Classical embeddings (TF-IDF, Word2Vec, GloVe, FastText)
- **LLM Adaptation**
  - OLMoE Instruct model fine-tuned with LoRA
- **Retrieval**
  - Vector similarity search using FAISS
- **Generation & Ranking**
  - Retrieval-Augmented Generation (RAG) with LangChain
- **Output**
  - Semantically ranked candidate recommendations with contextual relevance

## Insights
### From Keyword Matching to Semantic Understanding
  - Classical embedding methods captured surface-level similarity but struggled with contextual meaning
  - LLM-based representations enabled deeper semantic alignment between job requirements and candidate experience
  - The shift from keyword overlap to meaning-based matching significantly improved ranking relevance

### Role of LoRA Fine-Tuning
  - LoRA allowed efficient adaptation of a large language model without full fine-tuning
  - Fine-tuning improved domain alignment for recruitment-specific language
  - The approach balanced performance gains with computational efficiency
    
### RAG as a Structural Advantage
  - FAISS-based retrieval ensured scalability and fast similarity search
  - RAG decoupled knowledge retrieval from generation, improving controllability
  - The system remained flexible without dependency on external vector databases such as Pinecone

### LLM Behavior & Practical Trade-offs
  - LLM outputs were more robust to variations in phrasing and terminology
  - Increased model expressiveness came with higher inference cost
  - Retrieval quality directly influenced generation quality, highlighting the importance of embedding alignment

### Business & System-Level Takeaways
  - Semantic ranking improves candidate discovery in noisy, real-world hiring data
  - LLM-based systems are most effective when combined with structured retrieval
  - Efficient fine-tuning strategies are critical for practical deployment

## Outcome
  - Built a scalable semantic candidate ranking pipeline using LLMs
  - Demonstrated the effectiveness of LoRA fine-tuning and RAG for recruitment use cases
  - Established a foundation for production-ready, meaning-aware talent matching systems

## Technologies Used
  - Programming Language
    - Python
  - LLM & NLP
    - OLMoE Instruct
    - LoRA fine-tuning
  - Retrieval
    - FAISS
  - Frameworks
    - LangChain
  - Embeddings
    - TF-IDF, Word2Vec, GloVe, FastText

