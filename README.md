# MAS4115 Final Project: Analyzing Public Sentiments about AI on Twitter

## Project Link
[Colab Notebook](https://colab.research.google.com/drive/15gUETP0jje74U_O5fDcJ1mORtXzr0OKa?usp=sharing)

## Introduction
This project investigates public sentiments about ChatGPT and artificial intelligence (AI) on Twitter. Using a dataset from Kaggle that contains tweets over a one-month period, I applied linear algebra methods to gain insights into how AI is perceived. The goal is to provide researchers with conclusions about public attitudes towards AI and the evolving landscape of AI integration into society.

## Research Objectives
The primary research question driving this project is: *What are the predominant sentiments expressed about AI on Twitter, and what themes emerge from these discussions?*

Specific objectives:
1. Identify the overall sentiment trends (positive, negative, neutral) in AI-related tweets.
2. Detect recurring themes within AI discussions.
3. Apply linear algebra techniques (PCA and Truncated SVD) to visualize and interpret sentiment patterns.

## Dataset Overview
- **Source:** Kaggle dataset with 10,000 AI-related tweets
- **Sentiment Distribution:**
  - **Negative:** 49.16%
  - **Positive:** 25.54%
  - **Neutral:** 25.30%

## Data Analysis Approach

### Sentiment Analysis
- Used **NLTK's Vader Sentiment Analyzer** to compute sentiment scores for each tweet.
- Results suggested a more **mixed sentiment landscape** than the dataset's predefined labels indicated.
- The Vader-based analysis detected a blend of positive and negative sentiment signals in tweets classified as neutral, challenging the original dataset's sentiment labeling.

### Text Analysis Using Linear Algebra
To further explore sentiment structures, I applied:
1. **Principal Component Analysis (PCA):**
   - Reduced tweet vectors' dimensionality to visualize sentiment clusters.
   - Found that tweet length, rather than sentiment, played a major role in clustering.

2. **Truncated Singular Value Decomposition (SVD):**
   - Decomposed the TF-IDF matrix of tweets to identify dominant patterns.
   - Revealed distinct tweet clusters based on word importance rather than sentiment variation.

## Implementation Details
- **Technologies Used:** Python, NLTK, pandas, NumPy, matplotlib
- **Key Techniques:** Text preprocessing, sentiment scoring, dimensionality reduction

## Key Findings
- **Mixed Public Sentiment:** While media often portrays AI in a negative light, the Twitter sentiment landscape is more **diverse and mixed**, reflecting both enthusiasm and apprehension.
- **Recurring Discussion Themes:** Certain topics frequently appear in AI-related discussions, but the distribution of tweet lengths suggests that clustering is influenced by common tweet formatting rather than sentiment alone.
- **Limitations of Predefined Sentiment Labels:** Vader's analysis challenged the dataset's original sentiment classifications, emphasizing the need for more nuanced sentiment evaluation.

## Conclusion
This project demonstrates the power of **linear algebra and natural language processing (NLP) in analyzing large-scale sentiment data**. The findings indicate that public opinion on AI is more **nuanced and complex** than initially perceived. These techniques provide a scalable approach for researchers to study evolving sentiments on AI and other emerging technologies.

## Resources
- [NLTK Documentation](https://www.nltk.org)
- [Vader Sentiment Analysis GitHub](https://github.com/cjhutto/vaderSentiment)
- [Kaggle Dataset](https://www.kaggle.com/datasets/charunisa/chatgpt-sentiment-analysis/data)
- [PCA vs. SVD Overview](https://medium.com/@notsokarda/pca-vs-svd-simplified32c5c753998)

---
### How to Use This Repository
- Clone the repository: `git clone <repo-link>`
- Install dependencies: `pip install nltk pandas numpy matplotlib`
- Run the Colab notebook linked above to explore the sentiment analysis and visualizations.

**Author:** Ian DeLano

