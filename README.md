#  Web_Scraping_data_project

##Project Overview: 
  IPL Auction Data Scraper

  This project demonstrates how to extract structured data from a web page, process it using Python, and save it for further analysis. Specifically, it scrapes 
  data from the IPL 2023 auction page, processes the extracted table, and exports the results to an Excel file.

##Features:
  1.Web Scraping:
    Uses the requests library to fetch the HTML content of the IPL auction page.
    Employs BeautifulSoup from the bs4 library to parse the HTML and extract relevant table data.

  2.Data Processing:
    Extracts table headers and rows dynamically.
    Ensures consistency between the number of headers and row data to avoid mismatched entries.
    Logs mismatched rows to help debug issues with incomplete or malformed data.

 3. Data Storage:
    Utilizes pandas to structure the data into a DataFrame.
    Exports the processed data to an Excel file for easy sharing and analysis.
    Tools and Libraries Used:
    requests:

Facilitates HTTP requests to fetch the web page content.
Example: r = requests.get(url) retrieves the HTML source of the IPL auction page.
BeautifulSoup (from bs4):

Parses the HTML content and navigates the page structure.
Example: soup.find("table", class_="ih-td-tab") locates the target table.
pandas:

Provides a DataFrame structure to organize and manipulate the extracted data.
Example: df.to_excel() exports the DataFrame to an Excel file.
lxml:

A parser used by BeautifulSoup for efficient HTML and XML parsing.
Steps Performed:
Fetch Web Page:

The IPL auction page is downloaded using requests.
Parse and Locate Table:

The HTML is parsed using BeautifulSoup, and the target table is identified using its CSS class.
Extract Data:

Table headers (<th>) and rows (<tr>) are extracted, processed, and stored in a pandas DataFrame.
Export to Excel:

The resulting data is saved as ipl_Auction_data.xlsx, making it accessible for analysis.
