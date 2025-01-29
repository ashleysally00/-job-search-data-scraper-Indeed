
# Job Search Web Scraper for Indeed

## Project Origins
I made this while doing the "Scrape and analyze data analyst job requirements with Python" guided project on Coursera. You can create your own version of the project for free by enrolling [here](https://www.coursera.org/learn/scrape-job-postings-data-analyst/home/module/1).

## Project Overview
A Python-based job search data extraction tool that demonstrates web scraping, data processing, and CSV file handling. The project was developed using Jupyter Notebook and focuses on scraping job postings from Indeed.com.


### 1. URL Generation
- Takes position and location parameters
- Formats them for URL compatibility
- Creates properly structured URLs for job searches

### 2. Data Extraction
- Implements robust error handling with try/except blocks
- Extracts key job information (title, company, location, salary, description)
- Handles missing data gracefully

### 3. Main Program Flow
- Manages the complete scraping process
- Handles HTTP requests with appropriate headers
- Processes multiple job postings
- Saves data to CSV format

## Technical Challenges & Solutions

HTML Parser Selection
The project uses Python's built-in HTML parser. 

- It's built into Python (no additional installations needed)
- It's good enough for most web scraping tasks
- It's more lenient with malformed HTML than some other parsers


```python
import requests
from bs4 import BeautifulSoup

headers = {
    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36',
    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
    'Accept-Language': 'en-US,en;q=0.5',
    'Connection': 'keep-alive',
}

page = requests.get(url, headers=headers)
soup = BeautifulSoup(page.content, 'html.parser')

# Find job listings using the parser
job_cards = soup.find_all('div', class_='job_seen_beacon')
```
### Web Scraping Limitations
- Challenge: Indeed's anti-scraping measures blocked direct scraping
- Solution: Implemented a sample data version to demonstrate functionality
- Learning: Understanding real-world API limitations and alternative approaches

### Error Handling
- Implemented comprehensive try/except blocks
- Ensured program stability with missing data
- Created default values for missing fields

## Future Improvements
- Implement Indeed's official API integration
- Add support for multiple job boards
- Include pagination for multiple result pages
- Add data cleaning and deduplication
- Create visualization of job market trends
- Add email notifications for new postings

## Installation & Usage


## Technologies Used
- Python
- Jupyter Notebook
- BeautifulSoup
- Pandas
- Requests

## Sample Output
- **Job Search Results Processing** <br>
![Job Search Results](https://github.com/ashleysally00/job-search-web-scraper-Indeed/blob/main/snapshot_of_output1.png)

- **Job Posting Test Cases** <br>
![Job Posting Tests](https://github.com/ashleysally00/job-search-web-scraper-Indeed/blob/main/snapshot_of_output2.png)

- **CSV Data Export** <br>
![CSV Export](https://github.com/ashleysally00/job-search-web-scraper-Indeed/blob/main/snapshot_CSV.png)

