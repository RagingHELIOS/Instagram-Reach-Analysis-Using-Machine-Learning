# Instagram Reach Analysis Using Machine Learning

This project analyzes Instagram post reach using Python and Machine Learning techniques. It demonstrates how to clean and process data, explore relationships between metrics, and build a prediction model for estimating the reach of Instagram posts based on engagement factors.

## Features
1. **Data Cleaning and Exploration**:
   - Loaded and cleaned the dataset for missing values.
   - Explored various metrics like impressions, likes, comments, shares, and hashtags.
   
2. **Visualization**:
   - Distribution of impressions from sources like home, hashtags, and explore.
   - Pie charts for impressions breakdown.
   - Word clouds for captions and hashtags to understand content trends.

3. **Relationship Analysis**:
   - Scatter plots with trendlines to visualize relationships between:
     - Impressions and likes.
     - Impressions and comments.
     - Profile visits and followers gained.

4. **Correlation Analysis**:
   - Computed correlation coefficients to find the strongest predictors of impressions.

5. **Conversion Rate Analysis**:
   - Calculated the conversion rate from profile visits to follows.

6. **Machine Learning Model**:
   - Built a `PassiveAggressiveRegressor` model to predict impressions based on features like likes, saves, comments, shares, profile visits, and follows.
   - Achieved a model accuracy of ~90.7%.

## Libraries Used
- Data Analysis: `pandas`, `numpy`
- Visualization: `matplotlib`, `seaborn`, `plotly`, `WordCloud`
- Machine Learning: `sklearn` (Passive Aggressive Regressor, train-test split)

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Instagram-Reach-Analysis.git
   cd Instagram-Reach-Analysis
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
3. Run the script:
   ```bash
   python instagram_reach_analysis.py

## Key Insights
  - Impressions are heavily influenced by factors such as likes, saves, and profile visits.
  - "From Explore" and "Follows" show the highest correlation with impressions.
  - Word cloud analysis highlights the most used hashtags and caption keywords that engage users.

## Prediction Example
Using the trained model, you can predict the reach of an Instagram post based on its engagement metrics. Example input:

features = [[282, 233, 4, 9, 165, 54]].
predicted_reach = model.predict(features).

## Dataset
The dataset contains key metrics for Instagram posts, including:
  - Impressions from various sources (home, hashtags, explore, etc.)
  - Likes, saves, comments, shares
  - Profile visits and follows
  - Captions and hashtags

## Results
  - The model achieves an accuracy of 90.7% in predicting post impressions.
  - Insights derived from the analysis can help optimize Instagram content for better reach.

## Future Enhancements
  - Extend the analysis to include time-based trends.
  - Integrate sentiment analysis for captions and comments.
  - Experiment with advanced machine learning models like XGBoost or neural networks.
