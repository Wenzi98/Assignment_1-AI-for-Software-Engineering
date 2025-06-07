Assignmnent Overview
This repository contains a rule-based cryptocurrency advisor chatbot designed to be your first AI-powered financial sidekick! The bot analyzes predefined cryptocurrency data to provide investment advice based on profitability (price trends) and sustainability (energy efficiency, project viability).

Features
Rule-based decision making: Provides recommendations using simple if-else logic

Dual analysis: Evaluates both profitability and sustainability factors

Predefined dataset: Includes data for Bitcoin, Ethereum, and Cardano

Interactive: Responds to natural language queries about crypto investments

Dataset Structure
The chatbot uses the following predefined dataset:

python
crypto_db = {  
    "Bitcoin": {  
        "price_trend": "rising",  
        "market_cap": "high",  
        "energy_use": "high",  
        "sustainability_score": 3/10  
    },  
    "Ethereum": {  
        "price_trend": "stable",  
        "market_cap": "high",  
        "energy_use": "medium",  
        "sustainability_score": 6/10  
    },  
    "Cardano": {  
        "price_trend": "rising",  
        "market_cap": "medium",  
        "energy_use": "low",  
        "sustainability_score": 8/10  
    }  
}
How It Works
The chatbot responds to queries like:

"Which crypto is trending up?"

"What's the most sustainable coin?"

"Which crypto should I buy for long-term growth?"

Example logic:

python
if "sustainable" in user_query:  
    recommend = max(crypto_db, key=lambda x: crypto_db[x]["sustainability_score"])  
    print(f"Invest in {recommend}! 🌱 It's eco-friendly and has long-term potential!")
Installation
Clone this repository

Ensure you have Python installed (3.6+ recommended)

No additional dependencies required for basic version

Usage
Run the Python script and interact with the chatbot through the command line interface.

Stretch Goals (Optional)
Integrate with CoinGecko's API for real-time data

Implement NLP with NLTK for more natural language processing

Add ethical disclaimer about crypto risks

Ethical Note
⚠️ Remember: "Crypto is risky—always do your own research!" This bot provides educational suggestions only.

Submission Requirements
GitHub repo with:

README.md (this file)

Python script (.py file)

Screenshots of chatbot interactions

30-second screen recording of chatbot interaction

50-word summary explaining how the chatbot mimics basic AI decision-making

Learning Outcomes
✅ Understand basics of AI-driven decision-making
✅ Learn to design conversational logic
✅ Practice simple data analysis for crypto trends
