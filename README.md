## Apziva Projects — Overview
During my time at <b>Apziva</b>, I worked as a <b>Data Scientist / AI Resident</b>, focusing on solving real-world business problems using machine learning, NLP, and LLM-based systems.
My work focused on <b>end-to-end pipelines</b>, spanning data exploration and modeling through to evaluation and the generation of actionable insights.

<b>Key themes across projects</b>
- Real-world, industry-scale datasets
- Customer satisfaction and decision support
- Ranking and recommendation systems
- NLP, classical ML, and LLM integration
- Translating business questions into deployable ML solutions

<br>
<br>

|Number|Project Title|Description|
|------|---|---|
|1|Happy Customers|Built and evaluated classification models to predict customer satisfaction using survey data, and identified key drivers influencing service quality to support business decision-making|
|2|Term Deposit Marketing|Developed data-driven targeting and segmentation strategies to reduce call volume and improve subscription rates by addressing class imbalance and evaluating multiple predictive models|
|3|Potential Talents|Designed a semantic candidate ranking system using NLP embeddings, learning-to-rank techniques, and LLM-based retrieval to match job descriptions with relevant candidate profiles|
|4|MonReader|Implemented an end-to-end OCR and text-to-speech pipeline that extracts text from image batches, filters low-confidence results, and converts content into audio for improved accessibility|
|5|Value Investor|Explored data-driven approaches to value investing by analyzing financial indicators and market signals to support long-term investment decision-making|
|6|Voice Cloning and Fake Audio Detection|Investigated techniques for voice cloning and synthetic audio detection, focusing on identifying patterns and features that distinguish real and generated speech|
|7|Sales Reinforcer|Examined reinforcement-based strategies to support sales decision-making by modeling customer interactions and optimizing engagement policies|


<br>

### <b>1. Happy Customers — Customer Satisfaction Prediction</b>
<b>Goal</b><br>
Predict customer satisfaction levels and identify the key factors that influence service quality, enabling the business to prioritize operational improvements.
<br>

<b>What I Did</b><br>
- Conducted exploratory data analysis (EDA) on survey-based customer data
- Identified key satisfaction drivers through feature analysis
- Trained and tuned Logistic Regression and XGBoost models
- Achieved 74% accuracy, exceeding the business benchmark of 73%
- Translated model outputs into actionable business insights

<b>Skills & Tools</b><br>
- Python, scikit-learn, XGBoost
- Classification modeling
- Feature importance & evaluation


<br>

### <b>2. Term Deposit Marketing — Customer Targeting & Segmentation</b>
<b>Goal</b><br>
Reduce unnecessary call volume while improving subscription rates for a term deposit marketing campaign.
<br>

<b>What I Did</b><br>
- Addressed class imbalance using SMOTE, Tomek Links, and related techniques
- Performed customer segmentation using PCA, t-SNE, UMAP, and K-means clustering
- Trained and evaluated Logistic Regression, Random Forest, and Gradient Boosting models
- Compared models using F1-score and ROC-AUC
- Proposed data-driven targeting strategies that reduced call volume and improved conversion rates
- Visualized results using Tableau and shared insights via a presentation video

<b>Skills & Tools</b><br>
- Python, scikit-learn
- Dimensionality reduction & clustering
- Model evaluation & business-oriented reporting
- Tableau


<br>

### <b>3. Potential Talents — Candidate Ranking & LLM-Based Retrieval</b>
<b>Goal<b><br>
Enable recruiters to identify suitable candidates efficiently using semantic search and ranking instead of keyword matching.
<br>

<b>What I Did</b><br>
- Vectorized job descriptions and candidate profiles using TF-IDF, Word2Vec, GloVe, and FastText
- Implemented cosine similarity–based ranking
- Applied Learning-to-Rank approaches, including RankNet
- Fine-tuned the OLMoE-1B–7B Instruct model using LoRA for efficient adaptation
- Built a retrieval-augmented generation (RAG) pipeline using FAISS and LangChain (without Pinecone)
- Developed a semantic candidate ranking system and presented the project at Apziva’s Generative AI Workshop

<b>Skills & Tools</b><br>
- NLP & embedding models
- Learning-to-Rank
- LoRA fine-tuning
- FAISS, LangChain
- LLM-based retrieval systems

<br>

### <b>4. MonReader — OCR & Text-to-Speech Pipeline</b><br>
<b>Goal</b>
Automate text extraction from large batches of images and convert extracted text into speech for improved accessibility.

<b>What I Did</b><br>
- Built an OCR pipeline using EasyOCR
- Applied confidence-level filtering to remove noisy or low-quality text
- Converted recognized text into audio using Google Text-to-Speech (gTTS)
- Designed an end-to-end batch-processing pipeline for scalable use


<b>Skills & Tools</b><br>
- Python
- EasyOCR, gTTS
- Data preprocessing & pipeline design
