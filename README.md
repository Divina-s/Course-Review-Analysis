# Course Review Analysis and Visualization

## Repository Description
This project analyzes and visualizes course reviews from Coursera and Udemy to extract meaningful insights. By applying textual visualization techniques, such as word clouds, bar charts, sentiment analysis, and topic modeling, this project highlights user preferences and course feedback trends. The repository includes code for scraping, cleaning, analyzing, and visualizing user reviews.

---

## Project Overview

**Objective**: 
- Extract and visualize meaningful information from unstructured user review data using textual visualization techniques.
- Highlight key findings such as user satisfaction, popular topics, and trends in sentiment over time.

### Deliverables
- **Cleaned Dataset**: Reviews from Coursera (scraped) and Udemy (Kaggle dataset).
- **Textual Visualizations**: Word clouds, sentiment trends, bar charts, and topic modeling visualizations.
- **Final Report**: Document summarizing methods, results, challenges, and insights.

---

## Datasets
### **1. Udemy Dataset (Kaggle)**
- **Source**: [Kaggle Udemy Dataset](https://www.kaggle.com/datasets/hossaingh/udemy-courses)
- **Description**: Contains Udemy course reviews with fields such as `id`, `course_id`, `rate`, `date`, `name`, and `review`.

### **2. Coursera Dataset**
- **Source**: Scraped directly from Coursera using Python.
- **Description**: Reviews for selected Coursera courses, including fields like `id`, `course_id`, `rating`, `date`, `review`, and `name`.

---

## Tools and Libraries

### **Data Collection**
- `BeautifulSoup`: For scraping Coursera reviews.
- `requests`: For making HTTP requests to fetch web pages.

### **Text Preprocessing**
- `pandas`: For data cleaning and manipulation.
- `langid`: For detecting and filtering non-English reviews.
- `nltk`: For tokenization, stop-word removal, and lemmatization.
- `re`: For cleaning textual data using regular expressions.

### **Visualization**
- `matplotlib`: For creating static plots and bar charts.
- `seaborn`: For advanced statistical visualizations.
- `wordcloud`: For generating word clouds.
- `plotly`: For interactive visualizations.
- `pyLDAvis`: For visualizing topic modeling results.

### **Text Analysis**
- `gensim`: For topic modeling using Latent Dirichlet Allocation (LDA).
- `textblob`: For sentiment analysis.
- `scikit-learn`: For vectorization and other text-processing tasks.

---

## Methodology

### **1. Data Collection**
- Reviews were scraped from Coursera courses using `BeautifulSoup`.
- Udemy reviews were loaded from the Kaggle dataset.

### **2. Data Cleaning**
- Removed filler content (e.g., repeated phrases like "Filled Star").
- Filtered reviews to retain only English entries using `langid`.
- Reformatted dates for consistency and dropped irrelevant columns.

### **3. Analysis**
- **Sentiment Analysis**: Classified reviews as positive, neutral, or negative.
- **Keyword Analysis**: Extracted frequent words and themes from reviews.
- **Topic Modeling**: Used LDA to discover hidden themes across reviews.

### **4. Visualization**
- Created word clouds, bar charts, and sentiment trends to highlight findings.
- Used pyLDAvis for interactive exploration of topics in reviews.

---


