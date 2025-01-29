
# Job Search Web Scraper Indeed

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
[]
