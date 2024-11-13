# web-scrapping-and-reporting-tool
 Automated Web Scraping and Reporting Tool, this script will scrape data from multiple websites, aggregate the data, generate a report, and automatically email the report to a specified recipient.

code explaination:-

Web Scraping:
The scrape_website function sends a GET request to the website and uses BeautifulSoup to parse the HTML.
It extracts the article titles and links from the page (adjust the tags and attributes based on the structure of your target websites).
Data Aggregation:

The aggregate_data function combines the scraped data from multiple websites into a single pandas DataFrame for easy manipulation and reporting.
Report Generation:

The generate_report function saves the data as both a CSV and an HTML file, which will be sent as attachments in the email.
Emailing the Report:

The send_email function uses smtplib to send an email with the CSV and HTML report files attached.
You'll need to provide your email credentials for sending the email. If using Gmail, you might need to generate an App Password for better security instead of using your regular password.
Main Workflow:

The main function orchestrates the whole process: scraping, aggregating, generating the report, and sending the email.
