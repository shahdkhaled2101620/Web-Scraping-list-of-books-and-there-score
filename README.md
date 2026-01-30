# 📚 Goodreads Books Web Scraping Project

📌 Project Overview

This project demonstrates web scraping using Python to collect book data from Goodreads.
The data is scraped from two different Goodreads list pages, then cleaned, merged, ranked, and exported to Excel for analysis.

The goal of this project is to practice:

1.Web scraping with requests and BeautifulSoup

2.Data cleaning and transformation using pandas

3.Merging datasets from multiple sources

4.Exporting structured data to Excel


🌐 Data Sources
The data was scraped from the following Goodreads pages:

1.Goodreads Top 100 Highest Rated Books (10,000+ ratings)

https://www.goodreads.com/list/show/153860.Goodreads_Top_100_Highest_Rated_Books_on_Goodreads_with_at_least_10_000_Ratings

2.Books with One Million Ratings

https://www.goodreads.com/list/show/35080.One_Million_Ratings


🛠 Tools & Libraries Used
Python 🐍

requests – to send HTTP requests

BeautifulSoup (bs4) – to parse HTML pages

pandas – for data manipulation and cleaning

Excel (.xlsx) – for exporting results


📊 Extracted Data Fields

For each book, the following information is collected:

Title

Author

Score (number of ratings)


⚙️ Project Workflow

Send HTTP requests to Goodreads pages using custom headers.Parse HTML content with BeautifulSoup.Extract book details from HTML table rows.
Store scraped data in a Pandas DataFrame.Export data from each page into separate Excel files.Merge both datasets into a single file

Clean the data:

1.Remove unnecessary columns
2.Clean and convert score values to integers
3.Sort books by score (descending)
4.Add ranking column
5.Export final cleaned dataset to Excel


📁 Output Files

practis_webscraping.ipynb.xlsx → Page 1 raw data

practis_webscraping.ipynb2.xlsx → Page 2 raw data

books_merged.xlsx → Merged dataset

books_clean.xlsx → Final cleaned and ranked dataset ✅


🧹 Data Cleaning Steps

1.Removed extra index columns

2.Cleaned score text (removed "score:" and commas)

3.Converted score values to integers

4.Sorted books by score

5.Added a ranking column


📈 Final Result

The final Excel file (books_clean.xlsx) contains:

Ranked books based on score

Clean and structured data

Ready-to-use dataset for analysis or visualization
