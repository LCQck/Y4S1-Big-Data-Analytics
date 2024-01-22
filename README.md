# Y4S1-Big-Data-Analytics

## Table of Contents
1. [Project 1: Data Scraping](#project-1-data-scraping)
2. [Project 2: Machine Learning for Predicting Employee Attrition](#project-2-machine-learning-for-predicting-employee-attrition)

# Project 1: Data Scraping

### Contributor
- **Name**: Changqing Lin
- **ID**: 2039153

## Task 1: Data scraping

### Description
This task involves a complex process of scraping quotes from `http://quotes.toscrape.com`, parsing individual quote details, author information, and additional properties from associated Goodreads pages. The script employs Python's robust libraries including `BeautifulSoup`, `pandas`, `requests`, and `re` among others, to navigate, extract, and process the data.

### Implementation Details
- **BeautifulSoup**: Used for parsing HTML and navigating the DOM.
- **requests**: For making HTTP requests to the target URLs.
- **pandas**: For constructing and manipulating DataFrames for data analysis.
- **time**, **random**: To introduce delays in the scraping process, mimicking human interaction and preventing being blocked by the website.
- **ssl**: To bypass SSL certification verification.
- **urllib3**: To suppress InsecureRequestWarning warnings due to unverified HTTPS requests.
- **re**: For regular expression operations, particularly in data cleaning and extraction.
- **difflib**: Included but not directly used in the provided code snippets.
- **matplotlib**, **seaborn**: For data visualization purposes.
- **tqdm**: To provide a progress bar during the scraping process.
- **numpy**: Utility functions for numerical operations, although its direct use isn't shown in the snippets.
- **datetime**: To process and standardize date formats.

The process involves several functions:
- `get_page_soups()`: Retrieve and parse page content iteratively.
- `get_quote_details(soup)`: Extract quote-related information.
- `get_author_details(url)`: Scrape detailed author information.
- `scrape_quotes()`: Aggregate scraping functions and compile the complete dataset.
- `standardize_date(date_str)`: Standardize date formats within the data.

The final output is a CSV file containing the scraped data, which is also displayed using `quotes_df.head()`.

### Code Execution
The script execution is reflected in the output, showing a 100% progress bar completion using `tqdm`. The scraping process includes data standardization and cleaning, resulting in a well-structured dataset ready for analysis.

### Security and Ethical Considerations
The script handles SSL verification and suppresses warnings to ensure uninterrupted scraping. It also incorporates delays to mimic human-like access patterns, which is a considerate scraping practice to reduce the load on the server.

---

## Task 2: The Influence of Tag Combinations on Quote Authors' Follower Counts

### Introduction
Task 2 delves into the impact of tag combinations on the popularity of quote authors, as reflected by their follower counts on Goodreads. The research question addresses whether quotes associated with certain tags command a larger following.

### Methods
The analysis entails loading the previously scraped data and conducting a frequency analysis of individual tags and tag combinations. Various visualization techniques like bar charts, pie charts, heatmaps, histograms, and boxplots are utilized to interpret the data and identify patterns.

### Visualizations
The project includes visual representations of the data to enhance understanding and provide insights into tag popularity and its correlation with author followers. Visualizations are crucial in discerning the significance of tag combinations in relation to author popularity.

---

# Project 2: Machine Learning for Predicting Employee Attrition

## Introduction
This project focuses on leveraging Big Data analytics to predict employee attrition. Using a dataset of various employee characteristics, we explore several machine learning models to identify patterns and factors that contribute to employee turnover.

## Data Loading and Exploration
The data is loaded using Pandas, and preliminary data exploration is conducted to assess feature distributions and identify non-contributing features that can be removed.

# Load the dataset
data = pd.read_csv('path_to_train.csv')
data.head()
# Feature Engineering and Preprocessing

The dataset undergoes preprocessing where categorical variables are encoded using one-hot encoding, and irrelevant features are dropped to streamline the dataset for machine learning algorithms.

## Model Training

Several models are evaluated for their performance:
- Logistic Regression
- Random Forest
- Gradient Boosting
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Decision Tree
- Voting Classifier (ensemble method)

## Model Evaluation

Models are assessed based on accuracy, precision, recall, and F1-score metrics. Cross-validation is used to ensure robust evaluation.

## Results

The Voting Classifier, which combines predictions from multiple models, showed the highest accuracy and robustness, making it the preferred model for predicting employee attrition.

## Discussion

Pros and cons of various models are discussed, and the advantages of ensemble learning methods such as the Voting Classifier are highlighted.

## Conclusion

The application of ensemble methods in Big Data analytics proves to be highly effective in predicting employee attrition, demonstrating the potential of machine learning in HR analytics for organizational planning and management.

## Full Report

For a detailed methodology, comprehensive analysis, and insightful visualizations, please refer to the [full project report][(link_to_full_project_report)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/2039153_Changqing%20Lin%20Project%202%20Report.pdf) by Changqing Lin.

## Requirements

The requirements and specifications for Project 2 can be found in the [Project 2 Requirements][(link_to_project_2_requirements)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/Project%202%20Requirements.pdf) document.

## Source Code

The complete source code for all analyses, model training, and evaluations is available in the [Jupyter Notebook][(link_to_jupyter_notebook)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/2039153_Changqing%20Lin%20Source%20Code.ipynb).
### Discussions and Conclusion
The study's conclusion points towards a correlation between popular tag combinations and higher follower counts for authors. This suggests that tags play a role in author visibility on social media platforms, though they represent only one aspect of the multifaceted dynamics of online popularity.

