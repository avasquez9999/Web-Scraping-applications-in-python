##Project 1:

# Web-Scraping-applications-in-python
Web scraping  university data and movie data

#Description:

This script utilizes Python's Beautiful Soup library to scrape data from the IMDB website. It specifically targets the search results page for movies released in 2018 (https://www.imdb.com/search/title/?release_date=2018-01-01,2018-12-31&sort=num_votes,desc) and aims to gather information for movies with over 4,000 votes. The script extracts the following details for each qualifying movie:

Movie Title

Release Year

IMDB Rating

Metascore (if available)

Number of Votes

The script isolates the first search result container and then proceeds to extract each data point of interest.

Key Points:

Targets IMDB movies released in 2018.
Focuses on movies with 4,000+ votes.
Scrapes title, release year, rating, Metascore (optional), and vote count.
Utilizes Beautiful Soup for data extraction.

#Implementing Rate Limiting and Random Delays

To ensure ethical and sustainable web scraping practices, we've incorporated rate limiting and random delays into our script.

**Rate Limiting:**

By introducing a controlled delay between requests, we minimize the risk of overwhelming the target server and potentially triggering IP bans.
Python's time.sleep() function allows us to pause script execution for a specified duration.
Random Delays:

To further mimic human behavior and avoid predictable patterns, we'll utilize random.randint() to introduce variability in the delay time between requests.
This helps to distribute the load on the server and reduce the likelihood of detection.
