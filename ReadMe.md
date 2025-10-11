**Competitor App Review Analysis**

## **Overview : **
<b>This project is focused on conducting a competitor analysis using user review data from two different mobile applications listed on the Google Play Store. The analysis aims to compare competing apps in the same domain by extracting review data, utilizing NLP techniques, and identifying the primary drivers behind high or low ratings based on user comments and ratings.
</b>

## **Data Collection Library : ** 
<b>This project uses the google-play-scraper, a Python package that provides a user-friendly API for crawling the Google Play Store and retrieving app metadata and review information without external dependencies. google-play-scraper helps fetch review text, user IDs, scores, app versions, thumbs up counts, and review timestamps directly in Python, making it ideal for large-scale data analysis tasks.
</b>

## **Workflow : **
1. *Data Collection:* User reviews for two competitor apps are fetched using the google-play-scraper Python library.

2. *Data Processing:* Reviews, ratings, app versions, and other metadata are cleaned and structured for analysis.

3. *NLP Analysis:* Sentiment classification and topic modeling are applied to review text using Hugging Face transformers.

4. *Insights & Visualization:* Results are summarized and visualized to highlight why each app receives positive or negative feedback, identifying differentiators and recurring themes.

## **Getting Started : **

1. Install dependencies from requirements.txt.

2. Set target app IDs for scraping.

3. Run the data extraction notebook or script.

4. Process and analyze the data in subsequent notebooks using NLP transforms.

5. Explore the visualizations and conclusions in the reporting notebook.

# **Example Use Cases : **

1. Product Managers: Understand user pain points and areas for improvement.

2. Developers: Prioritize bug fixes and new features.

3. Marketers: Benchmark apps against key competitors and refine positioning strategies.

# **Feedback & Collaboration : **

Suggestions or questions? Open an issue or reach out:

 email: hetdave2502@gmail.com 
 LinkedIn: https://www.linkedin.com/in/hetdave200225/

