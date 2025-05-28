# 📚 Research Paper Recommendation System


An intelligent academic search tool that recommends relevant and recent research papers using semantic embeddings, keyword extraction, and a hybrid ranking algorithm. The system is designed to assist researchers in efficiently discovering foundational and cutting-edge publications from the arXiv repository.

## 🔍 Overview ##

**Challenge:** Traditional keyword-based academic search engines often miss conceptually relevant research and struggle with emerging trends.

**Solution:** A hybrid NLP-based recommendation system using transformer models and a recency-aware scoring mechanism.

**Key Features:**

Semantic search using all-MiniLM-L6-v2 embeddings

Temporal ranking to prioritize recent publications

Explainable results with keywords and formatted citations

CLI-based interactive search experience

## 🎯 Objectives

Address semantic mismatches in traditional academic search

Enhance relevance and recency in recommendations

Improve user trust with explainable AI features

## 🛠️ Tech Stack

**Language:** Python 3.8+

**Libraries:** feedparser, sentence-transformers, spaCy, scikit-learn, numpy

**NLP Models:**

all-MiniLM-L6-v2 for sentence embeddings

en_core_web_sm for linguistic processing

## 🧪 Features

**Semantic Paper Search:**

Accepts natural language queries

Retrieves papers via the arXiv API

**Hybrid Ranking:**

Combines semantic relevance (70%) and recency (30%)

Uses cosine similarity and logarithmic decay

**Keyphrase Extraction:**

Extracts top 5 noun phrases using spaCy

**Citation Generation:**

APA-style citations for each recommended paper

**User Interface:**

CLI interface for query, result selection, and detailed views

## 🧱 System Architecture

**Pipeline Layers:**

Input Layer: Query entry via CLI

Processing Layer: NLP pipeline + hybrid ranking

Output Layer: Top 5 recommended papers with metadata

In-Memory Processing:

No database needed

Uses Python dictionaries for runtime efficiency

## 📈 Evaluation & Results

**Query Success Rate:** 100% (25 diverse test queries)

**Average Relevance Score:** 0.612

**Average Recency Score: **0.841

**Combined Score:** 0.680

Top 5 Results per Query: Ensures clarity and avoids overload

## ✅ Performance highlights:

Reliable across both technical and conceptual queries

Transparent score presentation built user trust

Better than arXiv’s native search in balancing old vs. new research

## 🚀 Installation
bash
Copy
Edit
# Clone the repository
git clone https://github.com/<your-username>/research-paper-recommender.git
cd research-paper-recommender

# Install required dependencies
pip install -r requirements.txt

# Additionally, install NLP models

python -m spacy download en_core_web_sm
## 💡 Usage

python

Copy

Edit

from main import user_interface

user_interface()

The CLI will prompt you to enter a query and interactively explore recommended research papers.

