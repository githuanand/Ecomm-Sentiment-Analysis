# E-Commerce Consumer Insights & Recommendation Engine

**Developed by:** Anand Mohan Jha

**Project Type:** End-to-End Data Science & Analytics

---

##  Project Overview

This project analyzes over **23,000 customer reviews** from a Women’s E-Commerce dataset. The goal is to provide actionable business intelligence by identifying product failure points and building a machine learning pipeline to predict customer recommendations.

###  Key Business Questions:

1. Which product departments are underperforming in customer satisfaction?
2. What are the specific "pain points" (sizing, quality, etc.) mentioned in negative reviews?
3. Can we automate the identification of "at-risk" customers using NLP?

---

##  Tech Stack

* **Data Extraction & Logic:** SQL (`PandasQL`)
* **Data Manipulation:** Python (`Pandas`, `NumPy`)
* **Data Visualization:** `Seaborn`, `Matplotlib`, `WordCloud`
* **Machine Learning (NLP):** `Scikit-Learn` (TF-IDF Vectorization, Logistic Regression)

---

##  The Data Pipeline

### 1. SQL Business Intelligence

Using SQL syntax within Python, I performed deep-dive aggregations to find the "Price vs. Quality" sweet spot.

* **Insight:** The **"Trend"** department was identified as the lowest-performing category with an average rating of **3.81/5**.

### 2. Natural Language Processing (NLP)

I used `TfidfVectorizer` to convert unstructured text into numerical features. This process, known as **TF-IDF (Term Frequency-Inverse Document Frequency)**, allows the model to "understand" the weight of specific words like "disappointed" vs. "love."

### 3. Machine Learning Implementation

I trained a **Logistic Regression** model to predict whether a user would recommend a product based on their review text. This algorithm functions as a binary classifier, calculating the probability of a "positive" recommendation.

---

##  Key Visualizations & Results

### Customer Pain Points

*The Word Cloud reveals that "sizing," "fit," and "fabric" are the primary drivers for 1-star and 2-star reviews.*

### 📊 Visualizing Customer Pain Points
<img width="944" height="506" alt="wordcloud" src="https://github.com/user-attachments/assets/df2268df-25ba-4998-a797-3c154ce427f9" />





*The Word Cloud above highlights that "sizing" and "fit" are the most frequent complaints in negative reviews.*

### Model Performance

*The Confusion Matrix demonstrates the model's reliability in distinguishing between positive and negative sentiment with **90% accuracy**.*
### 📈 Model Performance Evaluation
<img width="518" height="393" alt="confusion_matrix" src="https://github.com/user-attachments/assets/911522d3-5f91-4ca4-aa3e-208d400ae422" />






*The Confusion Matrix confirms a 90% accuracy rate, showing high reliability in predicting customer recommendations.*
---

##  Business Recommendations

1. **Quality Control:** The "Trend" department requires a manual audit of sizing guides to reduce return rates.
2. **Automated Flagging:** Implement the ML model to flag "Non-Recommendation" reviews in real-time for immediate customer support follow-up.
3. **Inventory Optimization:** Double down on "Intimates" and "Bottoms" departments, which showed the highest organic recommendation rates.

---

##  How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/amjha29/Ecom-Sentiment-Analysis.git

```


2. **Set Up Environment:** Ensure you have `kaggle.json` or your API key set as an environment variable in your Colab or Local Jupyter environment.
3. **Execute the Notebook:** Open `E_Commerce_Sentiment_Analysis.ipynb` and run all cells.

---

##  Contact

**Anand Mohan Jha**
[LinkedIn](https://www.linkedin.com/in/anand-mohan-jha-55843924a/)

[Email](mailto:aj1001194@gmail.com)
