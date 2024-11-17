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


Extract Data:

Table headers (<th>) and rows (<tr>) are extracted, processed, and stored in a pandas DataFrame.
Export to Excel:

The resulting data is saved as ipl_Auction_data.xlsx, making it accessible for analysis.
