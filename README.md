# CommonwealthBank-IntroToDataScience-Forage

## Task 1: Data Analysis of Supermarket Transactions

### Overview:
I was provided with a **CSV dataset** containing three years of transactional data from Australian supermarkets. The task involved answering the following questions:

1. How many apples were purchased in cash across locations?
2. How much cash was spent on apples?
3. How much money was spent by non-member customers at the Bakershire store?

### Approach:
I used **Excel** to filter the dataset and applied the **SUM** formula to calculate the required values. The data was filtered based on specific criteria (e.g., apples, cash payments, Bakershire store, non-member customers) to get the accurate results.

### Final Output:
The analysis was documented in the file with the formulas used for transparency, and the file was submitted for review.

## Task 2: Anonymising a Customer Data Set

### Overview:
The task was to anonymise a dataset of sensitive customer information while retaining the useful and valuable information for analysis. The dataset, **mobile_customers.csv**, contained customer details collected from users who signed up for a mobile app in the last three years.

### Approach:
To anonymise the data, I followed these steps:

1. **Removed unnecessary columns**: I deleted irrelevant data such as names or credit card numbers that wouldn’t contribute to the analysis.
2. **Masked identifiable information**: I masked sensitive information like passport numbers and mobile numbers.
3. **Categorised personal figures**: I grouped personal data such as age and income into categories or brackets (e.g., 18-25, 26-35).

These anonymisation techniques ensured the privacy of individuals while retaining the useful data for the data scientists at InsightSpark.

### Final Output:
The anonymised data was saved as a CSV file and submitted for review, ready for further analysis.

## Task 3: Exploring the @CommBank Twitter Account and API

### Overview:
The task was to explore the publicly available data from the **@CommBank Twitter Account** and learn about the **Twitter API** to propose ways to extract valuable insights for business purposes.

### Approach:
1. **Familiarisation with Twitter Account**: I started by reviewing the publicly available information on the **@CommBank Twitter account** to understand the type of data shared.
2. **Exploring the Twitter API**: I reviewed the **Twitter API: Data Dictionary** to understand the kinds of data that can be scraped programmatically using a language like Python.
3. **Business Insights**: I studied the **Twitter: Build for Business** guide to gain insights into how data can be leveraged in a business environment, particularly for marketing or customer engagement purposes.

### Proposal:
I created a proposal outlining methods to use the data from the **@CommBank Twitter account** to extract key insights. These insights could help InsightSpark in improving customer engagement, sentiment analysis, and monitoring public perception.

The proposal was submitted as per the instructions for review.

## Task 4: Database Design for Twitter Data

### Overview:
Design a database to store tweets from **@CommBank Twitter Account**, including replies, retweets, and mentions.

### Design:
1. **Tables**:
   - **Tweets**: tweet ID, content, timestamp, user ID
   - **Replies**: reply ID, tweet ID, user ID, content
   - **Retweets**: retweet ID, tweet ID, user ID
   - **Mentions**: mention ID, tweet ID, user ID

2. **Primary Keys**:
   - **Tweets**: tweet ID
   - **Replies**: reply ID
   - **Retweets**: retweet ID
   - **Mentions**: mention ID

3. **Relationships**:
   - **Replies** → **Tweets** (tweet ID)
   - **Mentions** → **Tweets** and **Users** (tweet ID, user ID)
   - **Retweets** → **Tweets** (tweet ID)

This design ensures minimal redundancy, accurate data relationships, and supports future analysis.
