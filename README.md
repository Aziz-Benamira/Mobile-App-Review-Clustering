# Mobile App Review Analysis

## Project Overview
As a **Data Scientist** working for a mobile app company, this project focuses on analyzing **negative user reviews** from the Google Play Store. The primary goal is to uncover insights and categorize negative feedback to help the product team improve the app and address user concerns. The analysis leverages **NLP techniques** (using NLTK) and **K-means clustering** (using scikit-learn) to identify themes and patterns in the reviews.

## Key Objectives
1. **Preprocessing Text Data**  
   - Tokenize reviews.
   - Remove stop words and non-alphanumeric characters.
   - Save cleaned data in a DataFrame `preprocessed_reviews`.

2. **Vectorization using TF-IDF**  
   - Transform the preprocessed reviews into a TF-IDF matrix (`tfidf_matrix`) for further analysis.

3. **Clustering Negative Reviews**  
   - Apply **K-means clustering** to group the reviews into 5 categories.
   - Store predicted cluster labels in a list called `categories`.

4. **Identifying Main Topics**  
   - For each cluster, identify the most frequent term.
   - Save the results in a DataFrame `topic_terms` with the following columns:
     - Cluster Label
     - Identified Term
     - Frequency

## Dataset
The analysis is based on the `reviews.csv` dataset, which contains the following columns:

| Column Name  | Description                                  |
|--------------|----------------------------------------------|
| `content`    | Content (text) of each review.              |
| `score`      | User-assigned score for the review (1 to 5). |

The focus is specifically on **negative reviews** with scores of **1 or 2**.


## Files in the Repository
- `analyze_reviews.py`: Main script for preprocessing, clustering, and topic extraction.
- `reviews.csv`: Sample dataset with user reviews and scores.
- `requirements.txt`: List of required Python libraries.
- `README.md`: Project description and instructions.

## Key Libraries Used
- **scikit-learn**: For K-means clustering and TF-IDF vectorization.
- **NLTK**: For text preprocessing and stop word removal.
- **pandas**: For data manipulation and analysis.

## Results and Insights
By running the analysis, you will:
1. Identify the main categories of negative reviews.
2. Reveal frequent terms within each cluster to highlight potential problem areas.
3. Provide actionable insights for improving app features and user satisfaction.

## Contributing
Feel free to contribute to this project by submitting a pull request or reporting issues. Contributions are welcome to improve preprocessing, clustering techniques, or visualization of results.

