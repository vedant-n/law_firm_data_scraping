Law Firm Data Scraper
This Python script scrapes data from law firm profiles on Vault.com and integrates it with scores from the top 100 law firms rankings on Vault.com. The scraped data includes law firm names, addresses, contact information, number of attorneys, and scores.

Requirements:
Python 3.x
Libraries:
requests
beautifulsoup4
pandas

Install required libraries using pip:

pip install requests beautifulsoup4 pandas

Usage
Clone the repository:

Modify the urls, name_classes, address_classes, phone_classes, no_of_attorneys_classes, referers, score_url, score_referer, and score_class variables in scraper.py to suit your scraping needs.

Configuration
urls: List of URLs of law firm profiles on Vault.com.
name_classes: List of classes to locate law firm names on each profile page.
address_classes: List of classes to locate law firm addresses on each profile page.
phone_classes: List of classes to locate law firm contact information on each profile page.
no_of_attorneys_classes: List of classes to locate number of attorneys at each law firm on each profile page.
referers: List of referer URLs corresponding to each urls entry, used to simulate search engine referrals.
score_url: URL of the page containing top 100 law firms rankings on Vault.com.
score_referer: Referer URL used for fetching scores.
score_class: Class used to locate score elements on the score_url page.
Output
The script outputs a CSV file named law_firm_data.csv containing the scraped data including law firm names, addresses, contact information, number of attorneys, and scores.
