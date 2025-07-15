# 🚘 Sentiment Analysis of Public Perception on Self-Driving Cars using BERT and LDA

This repository contains the complete codebase, datasets, and outputs from our research project:  
**"Public Perception of Self-Driving Cars: A Sentiment Analysis of YouTube Comments Using BERT"**  
We analyzed over **80,000 YouTube comments** related to autonomous vehicle technologies to explore public sentiment, identify concerns and expectations, and uncover thematic trends using advanced Natural Language Processing techniques.

---

## 📌 Project Highlights

- 🔍 **Dataset**: 80,000 YouTube comments from videos related to self-driving cars and autonomous vehicles.
- 🧼 **Preprocessing**: HTML cleaning, stopword removal, lemmatization, and noise filtering using NLTK.
- 💬 **Sentiment Analysis**:
  - Rule-based sentiment tagging with **VADER**
  - Deep contextual sentiment classification using **BERT** (`cardiffnlp/twitter-roberta-base-sentiment`)
- 🧠 **Topic Modeling**:
  - Unsupervised topic discovery using **Latent Dirichlet Allocation (LDA)**
  - Human-interpretable topic labeling and visualization
- 📊 **Visualizations**:
  - Sentiment distribution bar/pie charts
  - Word clouds for sentiment and topic
  - Topic-wise sentiment breakdown
  - Year-wise sentiment trend analysis

---

## 📁 Repository Structure

```bash
.
├── comments.csv                    # Raw YouTube comments dataset
├── comments_with_sentiment.csv    # Output from VADER sentiment analysis
├── comments_with_bert_sentiment.csv # Output from BERT sentiment classification
├── Sentiment_Analysis.ipynb       # Complete Jupyter notebook (cleaned, final version)
├── lda_topic_visualization.html   # Interactive topic explorer using pyLDAvis
├── figures/                       # Exported plots and word clouds (optional)
└── README.md                      # This file
````

---

## 🛠️ Installation & Requirements

This project runs on **Python 3.8+** and is compatible with **Google Colab**.

Install all required packages:

```bash
pip install pandas nltk gensim pyLDAvis transformers wordcloud seaborn matplotlib tqdm
```

Download required NLTK data once:

```python
import nltk
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('omw-1.4')
```

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/samar-pratap-singh230/Youtube_Comments_Sentiment_Analysis.git
   cd Youtube_Comments_Sentiment_Analysis
   ```

2. Run the `Youtube_Comments_Sentiment_Analysis.ipynb` notebook step by step:

   * Perform data cleaning
   * Run BERT-based sentiment classification
   * Generate visualizations and LDA topic models

3. View the interactive topic model at:

   ```
   lda_topic_visualization.html
   ```

---

### 📈 Key Findings (Updated)

* Out of \~80,000 public comments, **neutral sentiment** was most dominant, comprising **\~44%** of total responses. These comments often presented fact-based observations, cautious optimism, or unresolved opinions.
* **\~40% of the comments expressed negative sentiment**, highlighting recurring concerns about self-driving cars related to **safety risks, technological immaturity, control issues, and ethical dilemmas**.
* **\~16% of comments were positive**, reflecting **public excitement about innovation, AI integration, convenience, and the future of autonomous transportation**.
* Topic modeling using **Latent Dirichlet Allocation (LDA)** revealed 5 key discussion themes:

  1. **Human vs. Machine Judgment**
  2. **Road Infrastructure & Readiness**
  3. **User Expectations & Demand**
  4. **Technical Malfunctions & Bugs**
  5. **Brand Perception and Media Influence**
* Sentiment breakdown across these topics shows that even positive discussions are often interwoven with underlying caution or skepticism, reaffirming the complexity of public perception around AVs.

---

## 📚 Citation

If you use this project or refer to it in your work, please cite:

```
"Public Perception of Self-Driving Cars: A Sentiment Analysis of YouTube Comments Using BERT", 2025.
```

---

## 👥 Contributors

* Samar Pratap Singh — [@samar-pratap-singh230](https://github.com/samar-pratap-singh230)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🌐 Acknowledgements

* [HuggingFace Transformers](https://huggingface.co)
* [NLTK](https://www.nltk.org/)
* [Gensim + pyLDAvis](https://radimrehurek.com/gensim/)
* YouTube Public Data API for comment extraction

---
