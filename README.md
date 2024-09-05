# Business Employee Expenses: Analysis & Modeling

## Summary

Managing employee expenses by hand can be a real headache. It eats up valuable time and keeps people in repetitive tasks instead of focusing on what really matters. Using technology that automates the tedious stuff can help to make the whole process smoother and more efficient. This isn't just about reducing paperwork; it's about helping teams shift their attention to the bigger financial picture and empowering them to make better decisions for the company.

## Objective

In this project we **analyse spending trends** based on dummy business expenses dataset and we propose a **Machine Learning predictive model** to determine the expenses that need human attention.

## Dataset

The dataset includes key expense features: 

- expense_id: unique system-wide expense identifier	
- team_id: unique system-wide department identifier
- expense_created_at: timestamp of when expense was created
- review_status: status of latest review
- purchase_type: type of purchase, online or in store
- amount_value: authorization amount value
- amount_currency: currency of authorization amount	
- merchant_country: merchant registered country
- has_note: if the user added a note to the expense
- category: category of expense

## Methodology

In the first part, we conduct a exploratory analysis developed in Python that includes the following steps:

- Load data
- Feature Engineering
  - Check missing values
  - Transform date column
  - Convert all currencies to EUR
- Analyse Spending over time
- What are the most common categories?
  - Lunch
  - Meals & drinks
  - Travel
  - Events
- How spendings are made: online or in store?
- Analysis by Team
- Where the company spends the most?
- Detect Ouliers: Unusual Expenses
- Conclusions

In the second one, we present the Spending Priority Scoring System, a **ranking model** to estimate the *priority to review* detecting automatically those expenses that needs human attention.

## Tools used

- **Python** for coding
- **Quarto** for storytelling and report management

Python libraries:

- **mizani.formatters** for label currencies in plotnine
- **pandas** for data manipulation
- **forex_python.converter**  as a currency converter
- **yahoo_fin.stock_info* to import Yahoo Stock historical data
- **datetime** to handle date and time operations
- **plotnine** for data visualization
- **sklearn** for modeling and feature preprocessing



