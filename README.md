# Kamalesh Pantra

Final-year Integrated M.Sc. Data Science student at PSG College of Technology, Coimbatore. I graduate in May 2027 and I'm looking for full-time ML / data science roles starting December 2026.

Most of my work is around retrieval and recommendation. I care a lot about the evaluation side: ablations, significance tests, and checking that an improvement is real before I claim it.

## Working on now

- **Predict-Verify-Recommend**, a sequential recommendation paper (in progress, details below)
- **StrangeStreet**, my final-year project

## Projects

**[Multihop RAG Evaluation](https://github.com/kamaleshpantra/Multihop-RAG-Evaluation)**
Multi-hop question answering on HotpotQA. Retrieval runs FAISS dense search and BM25 side by side, merges the rankings with reciprocal rank fusion, then reranks with a cross-encoder. That gets Recall@10 to 79.32%. I added query expansion and evaluated generation end to end too: 44% exact match and 0.5065 F1, with both local (Ollama) and cloud LLMs.
`FAISS` `BM25` `Sentence Transformers` `RRF` `Ollama` `Streamlit`

**Predict-Verify-Recommend** (research, ongoing)
A verification-aware framework for sequential recommendation. An MLP transition model and a learned safety verifier sit on top of a SASRec backbone and filter out anomalous user states before recommending. My SASRec reproduction on MovieLens-1M landed within 1% of the published numbers (HR@10 0.8168 vs 0.8245). The verifier flagged 37% of candidates as anomalous, and bootstrap significance tests showed no accuracy loss.
`SASRec` `MovieLens-1M`

**[StockPulse](https://github.com/kamaleshpantra/StockPulse)**
Short-term stock trend prediction. An LSTM over historical prices and rolling market features, combined with sentiment scored from Reddit posts (PRAW + VADER). Comes with a Streamlit dashboard and a Docker setup.
`PyTorch` `LSTM` `VADER` `PRAW` `Streamlit` `Docker`

**[StrangeStreet](https://github.com/kamaleshpantra/strangestreet)**
An anonymous social platform, built backend-first. The feed is ranked with a UCB1 multi-armed bandit, SBERT embeddings handle semantic similarity, and there's secure messaging on top of FastAPI and PostgreSQL.
`FastAPI` `PostgreSQL` `SBERT` `UCB1`

**Health Insurance Premium Prediction**
Smaller one: an end-to-end regression pipeline, XGBoost tuned with RandomizedSearchCV (R² 0.9938), served through a Streamlit app.

## Internships

**ICU Medical**, R&D Embedded Software Intern (Jun to Nov 2025, Chennai)
Validation work on IV pump software under IEC 62304. I wrote Python/pandas scripts that went through 5,000+ pytest logs and grouped recurring failures, which cut manual triage by about 60%. I also wrote pytest suites for safety-critical modules and put validation evidence into structured reports for audits.

**Learner Circle**, Tech Intern (May to Jun 2024, Chennai)
Built an interpretable classifier (Random Forest, XGBoost, SHAP) on 500+ student records. Error analysis and ablations brought misclassification down 23%.

## Stack

**Languages:** Python, SQL, C++
**ML / GenAI:** PyTorch, scikit-learn, XGBoost, Hugging Face, LangChain, PySpark
**Data / retrieval:** FAISS, PostgreSQL
**Everything else:** FastAPI, Streamlit, Docker, Git

## Contact

kamaleshlmv@gmail.com · [LinkedIn](https://www.linkedin.com/in/kamalesh-pantra-4544a5255/)
