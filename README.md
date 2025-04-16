# Voice of the Customer (VoC) Team Repository 

## 📌 Overview
Welcome to the Voice of the Customer (VoC) team repository. This is a python based code repository containing code, datasets, and documentation for analyzing customer feedback, survey responses, and other related data. It is structured to support data cleaning, exploratory analysis, visualization, and advanced modeling (e.g., natural language processing (NLP), predictive modeling).

## VoC Team CX Background 
Purpose for the creation of this code repository is to analyze open text response survey data for recurring GSA surveys such as the Employee Pulse Survey, Customer Loyalty Survey (CLS/ISS), Internal Partner Satisfaction Survey (IPSS) and website feedback. We aim to equip users with a suite of statistical methods for analyzing survey data, including descriptive statistics, data visualization, natural language processing and text analysis tools for thematic analysis and sentiment analysis. We aim to make this tool accessible and user-friendly, even for those with minimal data science and coding experience.

## Project Team
### Maintainers
Kai Cobb  
Jun Zhong
### Contributors
Genevieve Christensen  
Camille Tucker  
Liz Brodd  
Katherine Petway  
Alexander Lopez-Perez  
Dionne Cochran

For any questions, please reach out to the project maintainers or open an issue. 

## Repository Layout
```
Voice-of-the-Customer-Team-Analysis/  
│── data/			# Raw & processed datasets (DO NOT COMMIT sensitive data)  
│── notebooks/			# Jupyter Notebooks for analysis & exploration  
│── src/			# Python scripts for data processing & modeling  
│── reports/			# Summary reports & visualizations  
│── docs/			# Documentation & guidelines  
│── presentations/		# Slide decks and PDF templates  
│── tests/			# Unit tests for data pipelines & script  
│── .github/			# GitHub workflows (CI/CD, issue templates, PR templates)  
│── requirements.txt		# List of dependencies  
│── CONTRIBUTING.md		# Contribution Guidelines
│── README.md			# Project overview & setup guide  
│── LICENSE			# License information
```


## Setup Instructions
Prerequisites & Requirements
Ensure you have the following installed:  
- Python (>=3.8)  
- Git  
- Virtual Environment (e.g., venv, conda)  
- Important packages/frameworks utilized include [Gensim](https://pypi.org/project/gensim/), [Numpy](https://numpy.org/), [Pandas](https://pandas.pydata.org/), [spaCy](https://github.com/explosion/spaCy), [NLTK](https://www.nltk.org/), [pyLDAvis](https://pypi.org/project/pyLDAvis/), [tqdm](https://github.com/tqdm/tqdm), [matplotlib](https://matplotlib.org/), [TextBlob](https://textblob.readthedocs.io/en/dev/), [seaborn](https://seaborn.pydata.org/), [sklearn](https://scikit-learn.org/stable/)
### Installation Steps
**1. Clone the repository**

```
git clone https://github.com/GSA/Voice-of-the-Customer-Team.git
cd Voice-of-the-Customer-Team
```

**2. Create a virtual environment**

```
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

**3. Install dependencies**

```
pip install -r requirements.txt
```

## Key Features
**Data Cleaning & Processing:** Scripts for handling missing values, text processing, and standardization. 
 
**Exploratory Data Analysis (EDA):** Jupyter notebooks with visualizations and statistical summaries.  

**Survey Response Analysis:** Custom scripts for sentiment analysis, topic modeling, and response categorization. 
 
**Reporting & Visualization:** Automated report generation with visual insights.

## Security & Data Handling
### 🚨 IMPORTANT GUIDELINES🚨
**DO NOT commit raw customer data** to the repository.
Never hardcode credentials in code. Hardcoding credentials (e.g., API keys, database passwords) directly into source code is a major security risk. 
Store sensitive configurations (e.g., API keys, database credentials) in **environment variables.**  
**Best Practice: Use Environment Variables**

***Instead of writing credentials directly in your code like this:***

```
DB_PASSWORD = "SuperSecret123"  # ❌ BAD PRACTICE
```

***Use environment variables:***

```
import os
DB_PASSWORD = os.getenv("DB_PASSWORD")  # ✅ GOOD PRACTICE
```

***Then, store the credential securely in an .env file or secret management system:***

```
DB_PASSWORD=SuperSecret123
```

***And load it using a library like dotenv:***

```
from dotenv import load_dotenv
load_dotenv()
```

## Contribution Guidelines
See the [Contribution Guidelines](https://github.com/GSA/Voice-of-the-Customer-Team/blob/main/CONTRIBUTING.md) file for more information.

## License
See the [LICENSE](https://github.com/GSA/Voice-of-the-Customer-Team/blob/main/LICENSE.md) file for details.




