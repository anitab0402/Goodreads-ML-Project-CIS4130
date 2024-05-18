# Goodreads-ML-Project-CIS4130

# Project Description
This project aims to analyze Goodreads book reviews to uncover trends in user ratings. The analysis includes exploratory data analysis,data cleaning, preprocessing, feature engineering, and predictive modeling.

# Objectives
- Develop predictive models to forecast book ratings based on review texts and other features.
- Visualize key insights and trends from the data.

# Dataset
The dataset used for this project is two JSON file named `goodreads_reviews_dedup.json`, `goodreads_books.json` which contains user reviews and ratings for various books on Goodreads extracted via Kaggle

## Data Processing Pipeline
The data processing pipeline includes the following steps:
1. **Data Collection**: Reading the dataset in chunks due to its large size.
2. **Data Cleaning and Preprocessing**:
    - Handling missing values.
    - Dropping unnecessary columns (`n_votes`, `n_comments`).
    - Converting columns to appropriate data types ex: (`book_id`, `rating`).
    - Formatting date columns (`date_added`, `read_at`, `started_at`) to `YY-MM-DD`.
3. **Feature Engineering**: Creating new features and transforming existing ones.
4. **Text Processing**: Using RegexToxenizer and Hashing
5. **Feature Scaling**: Applying `MinMaxScaler` to normalize numerical features.
6. **Pipeline Construction**: Building a data processing pipeline.

## Results and Findings
- Significant correlation between review length and rating.
- Predictive model achieved an RMSE of X and R-squared of Y.
- Visualizations included bar charts and scatter plots to highlight key trends.
- Best Model tested achieved an AUC of 0.837
