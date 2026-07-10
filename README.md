# News Classification: Automated Analysis of Conflict Narratives

**Automated classification of military, diplomatic, and humanitarian narratives in global news using Natural Language Processing and Deep Learning**

## Business Problem

Understanding how media frames global conflicts is critical for policymakers, intelligence agencies, and humanitarian organizations. This project builds an automated classification system to distinguish between military-focused, diplomatic-focused, and humanitarian-focused coverage in international news, enabling real-time monitoring of media narratives at scale.

**Key Applications:**
- Policy decision support for government agencies
- Media bias detection and analysis
- Early warning systems for humanitarian crises
- Strategic communications planning

## Project Overview

Analyzed 241 news articles from 16 international sources covering contemporary conflicts (Ukraine/Russia, Israel/Hamas, China/Philippines). Compared supervised classification (DistilBERT) with unsupervised topic modeling (LDA) to identify the most effective approach for automated framing detection.

## Technical Approach

**Data Collection:**
- RSS feed scraping from 16 international news sources (Al Jazeera, Reuters, BBC, Guardian, etc.)
- Keyword-based filtering across 3 categories (169 total keywords)
- Text preprocessing pipeline with HTML cleaning and normalization

**Methods:**
- **Supervised Classification:** Fine-tuned DistilBERT transformer model
- **Unsupervised Analysis:** Latent Dirichlet Allocation (LDA) topic modeling
- **Evaluation:** Accuracy, F1-score, precision/recall metrics

**Tech Stack:**
- Python, Pandas, NumPy
- Hugging Face Transformers (DistilBERT)
- Scikit-learn
- Natural Language Processing (NLP)

## Key Results

**Model Performance:**
- **Overall Accuracy:** 65.3% (7.6 points above baseline)
- **Diplomatic Coverage:** 67% precision, 93% recall
- **Military Coverage:** 60% precision, 38% recall
- **Macro F1-Score:** 41.3%

**Key Insights:**
- Supervised learning (DistilBERT) outperformed baseline for dominant frame types
- LDA revealed geographic clustering patterns rather than thematic frames
- Framing patterns are conflict-specific, not universal
- Class imbalance significantly impacts minority class detection

## Technical Highlights

- Built complete ML pipeline from data collection to model evaluation
- Fine-tuned state-of-the-art transformer model (DistilBERT)
- Handled real-world challenges: class imbalance, noisy data, overlapping categories
- Compared supervised vs unsupervised approaches systematically
- Optimized training time (reduced from hours to 5 minutes)

## Repository Contents

- `Adv_Analytics_Final (2).ipynb` - Complete analysis notebook with code, visualizations, and results
- `conflict_news_dataset_241.csv` - Dataset of 241 labeled news articles
- `README.md` - Project documentation (this file)

## Challenges & Learnings

**Challenges Addressed:**
- **Class Imbalance:** 57.7% diplomatic, 32.8% military, 9.5% humanitarian articles
- **Overlapping Terminology:** Many terms appear across multiple frame types
- **Geographic Variation:** Conflict-specific framing patterns
- **Technical Issues:** Debugged training loops, optimized model configuration

**Key Learnings:**
- Importance of balanced training data for minority class detection
- Context matters: geographic and cultural factors shape media framing
- Model performance varies significantly across frame types
- Need for conflict-specific training or transfer learning approaches

## Future Improvements

- Collect larger, more balanced dataset with stronger humanitarian representation
- Implement multi-label classification for overlapping frames
- Develop context-aware models incorporating geographic/temporal factors
- Expand to non-English sources for global perspective
- Deploy as real-time classification API

## About

Graduate project from Duke University's Master of Quantitative Management in Business Analytics program (May 2026). Demonstrates expertise in NLP, deep learning, and practical application of machine learning to real-world policy and intelligence problems.

**Technical Skills Demonstrated:** Python, Natural Language Processing, Deep Learning (Transformers), Data Collection & Preprocessing, Model Evaluation, Problem-Solving

## Connect

- LinkedIn: www.linkedin.com/in/beatriz-lassise2026


---
