# Y4S1-Big-Data-Analytics
2 Projects in INT303 Big Data Analytics:
Project 1: Data Scraping;
Project 2: Machine Learning for Predicting Healthcare Employee Attrition;
# Project 1: Data Scraping

## Task 1: Data scraping

### Contributor
- **Name**: Changqing Lin
- **ID**: 2039153

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

### Discussions and Conclusion
The study's conclusion points towards a correlation between popular tag combinations and higher follower counts for authors. This suggests that tags play a role in author visibility on social media platforms, though they represent only one aspect of the multifaceted dynamics of online popularity.

