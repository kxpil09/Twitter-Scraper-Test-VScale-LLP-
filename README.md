# Twitter Scraper Project
This project is a Twitter scraper that extracts data from specific tweets and saves the results to a CSV file. It utilizes the gspread library to access Google Sheets, the snscrape library for Twitter scraping, and the pandas library for data manipulation. The goal of the project is to gather information from influencers' tweets and related promoter tweets, storing relevant details such as timestamps, usernames, tweet URLs, and tweet texts in a structured format.

# Installation
* To run the Twitter scraper project, follow these steps:

* Clone the repository or download the source code.

* Install the required libraries using pip: 
  ``` pip install gspread oauth2client snscrape pandas``` 

* Replace the "file.json" file with your own Google Sheets credentials JSON file.

* Modify the URL in open_by_url to your specific Google Sheets URL.

* Run the script:
 ```python scraper.py```

* The output will be saved in a CSV file named "output.csv" and printed in the terminal.

# Usage
* Set up the Google Sheets credentials by providing the appropriate JSON key file.

* Ensure that your Google Sheets document contains Twitter links in the desired column.

* Configure the code to extract the desired number of Twitter links by modifying the range of values in the col_values function.

* Run the script to start scraping Twitter for the specified links.

* The script will scrape the influencer's tweet and, if available, the first promoter tweet related to the influencer and the link.

* The extracted data, including timestamps, usernames, URLs, and tweet texts, will be stored in a pandas dataframe.

* The resulting dataframe will be saved to a CSV file named "output.csv".

* The dataframe will also be printed in the terminal.

# Output
The code extracts data such as timestamps, usernames, tweet URLs, and likes from both the influencer and promoter tweets. If no tweet is found, an empty row is added. The final output is a CSV file named "output.csv"
![image](https://github.com/kxpil09/Twitter-Scraper-Test-VScale-LLP-/assets/99945815/be2baba2-c91f-4e47-84e0-1a70c85b0765)


# Credits
This project uses the following libraries:

* gspread
* oauth2client
* snscrape
* pandas
# Configuration
Before running the script, ensure that you have set up the necessary credentials for Google Sheets. Replace the "file.json" file with your own JSON key file containing the required access permissions.

# Contributing
Contributions to this project are welcome. If you would like to contribute, please follow these guidelines:

* Fork the repository.
* Create a new branch for your feature or bug fix.
* Make your changes and ensure that the code passes any relevant tests.
* Submit a pull request, explaining your changes and their purpose.
