# Ad Recommendation Pipeline Demo – T5 + XGBoost

This project demonstrates a simplified, research-style ad recommendation system simulating a real-time pipeline. It showcases retrieval, reranking, and scoring — commonly used in large-scale recommendation engines.

# Problem Overview

How can we recommend the most relevant ads to a user based on their query and profile in real time?

---

# Pipeline Summary

1. **User Embedding Generation (T5-style):**  
   Simulated using random vectors to mimic contextual embeddings for a user query.

2. **Top-K Ad Retrieval (Milvus-style):**  
   Cosine similarity is used to retrieve the most relevant ad embeddings from a pool.

3. **Feature Engineering for Reranking:**  
   Combines user profile features, ad metadata, and embedding similarity.

4. **XGBoost Reranking:**  
   A trained XGBoost classifier ranks the retrieved ads based on predicted relevance.

5. **Visualization:**  
   Bar chart shows predicted relevance scores of top ads.

---

# Tech Stack

- **Vector Similarity:** Cosine distance (simulated retrieval)
- **Embeddings:** Random vectors simulating T5 output
- **Reranking Model:** XGBoost classifier
- **Tools:** Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib
- **Vector DB Concept:** Simulated Milvus-style ANN retrieval


---

# Sample Output

text
Top recommended ads: ['ad_12', 'ad_7', 'ad_23', 'ad_5', 'ad_19']



ad-recommendation-pipeline-demo
├── README.md              # Project summary
├── pipeline_demo.ipynb    # Main notebook with full pipeline logic
└── requirements.txt       # Dependencies


Note
This is a simplified demo using randomly generated embeddings and features. It is designed to showcase the architecture and logic of a ranking system, not actual production metrics.
While Milvus is not directly used, the pipeline simulates its behavior using cosine similarity on embedding vectors.
