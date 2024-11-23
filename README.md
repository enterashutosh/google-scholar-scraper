# Google Scholar Profiles Scraper

This project is a web scraping tool built using Python and Selenium to extract detailed profiles of professors from Google Scholar. The script is designed to navigate through Google Scholar pages, avoid bot detection, and scrape comprehensive data fields while emulating human behavior.

## Features

- **Data Extraction**:
  - **Textual Profile Details**:
    - Professor Name
    - Affiliation
    - Most Cited Paper
    - Research Fields
  - **Citation Metrics**:
    - Total Number of Citations
    - h-index
    - i10-index
- **Cookie Management**: Uses preloaded cookies to bypass CAPTCHA challenges and bot detection.
- **Human-Like Behavior**: Simulates mouse movements, scrolling, and delays to mimic real user interaction.
- **Dynamic Interaction**: Automates search, profile selection, and data scraping using Selenium.
- **Randomized User-Agent**: Incorporates the `fake-useragent` library to randomize HTTP headers for better anonymity.

## Libraries and Tools Used

- **Selenium**: For web interaction and automation.
- **Pandas**: For storing and processing scraped data.
- **Fake-Useragent**: To generate randomized browser headers.
- **Chrome Developer Tools**: To inspect cookies, application layers, and web elements.
- **Google Scholar**: Target website for data scraping.

## Prerequisites

1. **Python 3.8+**
2. **Google Chrome** installed on your system.
3. **ChromeDriver** compatible with your Chrome version.
4. Required Python libraries:
   `pip install selenium pandas fake-useragent`

## Setup and Usage
1. Populate the `Scholars_list` in the script with professor names.
2. Set up valid cookies in the `cookies` variable.
3. Run the script:
   `python google_scholar_scraper.py`
4. Data is saved in `professor_profiles.csv`.

## Example Output

Professor Profiles Scraped:

| Professor Name | Affiliation         | Total Citations | h-index | i10-index | Most Cited Paper        | Research Fields       |
|----------------|---------------------|-----------------|---------|-----------|-------------------------|-----------------------|
| Cass Sunstein  | Harvard University  | 125,000         | 150     | 200       | Nudging: A Guide to...  | Behavioral Economics, Law |
| Tom Tyler      | Yale University     | 80,000          | 120     | 140       | Procedural Justice      | Social Psychology      |
| Mark Lemley    | Stanford University | 60,000          | 100     | 110       | Intellectual Property   | Law, Technology        |


## License

This project is not licensed for commercial use and is intended solely for educational purposes. The use of this script for scraping data from Google Scholar must comply with Google's Terms of Service. The author takes no responsibility for any misuse of this project.



