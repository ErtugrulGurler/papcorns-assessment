# Papcorns Data Scientist Technical Assessment

Welcome to Papcorns' Data Scientist technical assessment! This task is designed to evaluate your skills in data analysis, SQL, Python, and machine learning.

## Dataset Description

You are provided with a SQLite database (`papcorns.sqlite`) containing two tables:

### Users Table
- `id`: Unique identifier for each user (numeric)
- `created_at`: User creation timestamp (ISO date string)
- `attribution_source`: User acquisition source (tiktok, instagram, or organic)
- `country`: User's country (US, TR, or NL)
- `name`: User's name

### User Events Table
- `id`: Unique event identifier (numeric)
- `created_at`: Event timestamp (ISO date string)
- `user_id`: Reference to users table (numeric)
- `event_name`: Type of event (app_install, trial_started, trial_cancelled, subscription_started, subscription_renewed, subscription_cancelled)
- `amount_usd`: Transaction amount in USD (numeric)

## Tasks

Please complete the following tasks using Python and SQL. You can use any libraries you're comfortable with, but make sure to explain your approach and methodology.

### Core Tasks

1. Calculate the total revenue generated from subscriptions for each country.
2. Calculate the total number of trials given to users who came from Instagram.
3. Create a new column named 'acquisition_channel' by categorizing users based on their 'attribution_source':
   - 'Paid': users from instagram or tiktok
   - 'Organic': users from organic sources
4. Analyze the trial-to-subscription conversion rate:
   - Calculate the overall conversion rate
   - Break down the conversion rate by attribution_source
5. Calculate the median subscription duration (in months) for each country
6. Calculate the Average Lifetime Value (LTV) by country

### BONUS Tasks (Optional)

7. Predict the churn probability for user #1002 (Clark Kent)
   - Use any relevant features from the dataset
   - Explain your model selection and feature engineering process
   - Provide confidence intervals if applicable

8. Predict the potential Lifetime Value (pLTV) for user #1001 (Bruce Wayne)
   - Explain your methodology and assumptions

## Evaluation Criteria

Your submission will be evaluated based on:

1. **Code Quality**

2. **Analysis Quality**

3. **Communication**

## Submission Guidelines

Please provide:
1. Fork or create a new repository based on this template
1. A Jupyter notebook or Python script with your analysis
2. SQL queries used (if written separately)
3. Comment on code or a brief report explaining your approach and findings
4. If any assumptions made during the analysis
5. Send us the link to your repository back to dev+interview@papcorns.com

Good luck!
