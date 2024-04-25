# Cashback Scraper

## Overview
This a series of Python scripts, i.e: `scrape_discover_it_scrapper.py`, designed to scrape cashback deals from various credit cards. 
This tool is a small part of a system I'm developing to automate the process of collecting cashback opportunities, 
making it easier for users to find and take advantage of the best deals.

Another part of this system deals with insertion into a postgreSQL database. For example the `insert_discover_it.py` script is designed to 
insert cashback deals data into a database or a data structure after being scraped by the `scrape_discover_it_scrapper.py` script. 
As mentioned before, this tool is part of a larger system that helps users to manage and utilize cashback offers more efficiently.

Continuing with the theme of "parts of a whole system", error notification is sent using the function `send_email()` within 
`email_scrape_failed.py`. This file and function is found within the extra folder. 

Lastly, scripts like `create_discover_it_json.py` is designed to create and pass along strings using a JSON representation of HTML, URLs, 
file and folder names, keywords, etc. 

## Features
- Automated scraping of various credit cards with cashback offers.
- Extraction of deal details such as cashback percentage, merchant name, and offer validity.
- Inserts scraped cashback offer data into a specified database.
- Ensures data integrity and avoids duplicates.
- Can be integrated with other systems to enhance functionality.
- Error logging for failed email scraping attempts.
- JSON representation of strings to pass along as parameters or variables. 
- Notification system to alert of scrape failures.
- Easy-to-use interface for quick access to cashback information.

## Requirements
- Python 3.x
- Required Python packages: `requests`, `beautifulsoup4`, `lxml`

## Installation
To use the scraper, you need to have Python installed on your system. If you don't have Python installed, you can download it from python.org.

Once Python is installed, you can install the required packages using `pip`:
