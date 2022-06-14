# job-scraping-indeed
A web scraper to extract job postings from www.indeed.com

Created a data set using web scraping technique from the indeed.com website 
The Job title used is full time and the location is India
The information which is scraped from the website is as mentioned below
	Job title
	Company name
	Job posting date
	Salary range
	Job summary
	Job URL and
	the day which the data is scraped
1200+ records are scraped from the website

Libraries used:
	Requests - This library is used for sending HTTP request to a web page, it returns a Response object with all the data from web page
	BeautifulSoup - This is used to parse the HTTP returned response object in a tree like structure so that we can extract required data from the response object easily
	Pandas - To build the dataFrame
	Datetime – To return the date and time during which the data is scraped

Approach:
	Initially the URL of the website which needs to be scraped is taken and it was made more generalizable by which we can feed whichever job title and location we need
	Then request is made to URL and it returns the response with [200]
	BeautifulSoup is used  to navigate html tree structure other webpage and extract the relevant parts
	Class 'job_seen_beacon' with the tag 'div' contains all the collection of job posting on this page returning this would result in the collection of job postings
	Prototyping with respective single record is made
	By using the dot notations and tags to navigated through the tree structure
	Then all the required information is scraped with the help of HTML classes and tags and appended into a list and then into a file which is created which is further formed into a pandas DataFrame with required columns


![ak](https://user-images.githubusercontent.com/89577904/173627323-94bc43d2-2f44-403a-97a1-059eac842cd8.png)
