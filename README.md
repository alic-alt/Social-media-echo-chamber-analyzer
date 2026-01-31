# Social-media-echo-chamber-analyzer
Detecting echo chamber effects in Reddit using NLP and clustering.


# Social Media Echo Chamber Analyzer

## Project Overview
This project analyzes Reddit posts to detect **echo chamber effects** in online communities. Using natural language processing (NLP) and unsupervised machine learning, the project clusters posts based on linguistic similarity to identify concentrated or polarized discourse.

---

## Methodology

1. **Data Collection**
   - Two datasets are included:
     - `reddit_raw_posts.csv` — raw Reddit posts
     - `reddit_enriched_posts.csv` — enriched posts with preprocessing features like detected language, sentiment, and engagement metrics

2. **Data Preprocessing**
   - Removed posts with missing or empty text  
   - Standardized column names (`text` for post content, `engagement` for score)  
   - Sampled a subset of posts for analysis  

3. **Feature Extraction**
   - Applied **TF-IDF vectorization** to convert text into numerical features  

4. **Clustering**
   - Used **KMeans clustering** to group posts with similar linguistic content  
   - Reduced dimensionality with PCA for visualization  

5. **Analysis**
   - Measured **echo chamber tendencies** by analyzing clusters’ composition  
   - Visualized clusters and engagement patterns  

---

## Key Results
- Identified dominant conversational clusters within Reddit threads  
- Visualized echo chamber structures using PCA scatter plots  
- Observed differences in engagement and tone across clusters  


---

## Tech Stack
- Python 3  
- pandas, numpy  
- scikit-learn (TF-IDF, KMeans, PCA)  
- matplotlib (visualization)  
- nltk, textblob, langdetect (NLP preprocessing)  

---

## Repository Structure


