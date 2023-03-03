# Scraping-stackoverflow-using-Scrapy


Questions 1-4 have to be done using scrapy shell
Question 5 has to to executed using scrapy runspider spider_file.py -o outputfile_name -t file_extension
Question 1
From the given Stackoverflow page, extract all the questions listed on the page.

url = https://stackoverflow.com/questions
Note: Question 1 & 2 require the same page to be loaded. It is better you do not close the shell

Question 2
Request the page in Question 1 (or use the same shell) and fetch the hyperlink of each question listed on the page.

Question 3
This is question is similar to the previous questions

Go to the given Stackoverflow (jobs) page and extract the titles/role of all the jobs listed on the page.

url =  https://stackoverflow.com/jobs/companies
Note: Question 3 & 4 require the same page to be loaded. It is better you do not close the shell

Question 4
Request the page in Question 3 (or use the same shell), fetch the location of all the jobs posted on the given page.

Question 5
Write a spider to fetch details of the jobs listed on Stackoverflow jobs page. The details to be fetched are: Job title, Company, Location of the job. All the results must be written to a CSV file name jobs.csv.

The required Item class would be:

class JobItem(scrapy.Item):
    # Data structure to store the title, company name and location of the job
    title = scrapy.Field()
    company = scrapy.Field()
    location = scrapy.Field()
The link to Stackoverflow jobs page is: https://stackoverflow.com/jobs/companies

Question 6
In Question 5, you have stored all the jobs listed on the first page. Now, add page following capability to the spider you have just written. There are approximately 108 pages of job listing on the website: https://stackoverflow.com/jobs/companies.

Crawl all the pages and store all the jobs postings to a CSV file.
