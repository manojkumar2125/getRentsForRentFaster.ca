

# RentFaster.ca Data Scraper

## Overview

This project is designed to scrape rental listings data from **RentFaster.ca** and export all relevant details into a structured Excel spreadsheet for easy analysis and record-keeping.

## Features

* Automatically extract rental property information from RentFaster.ca.
* Collect key details such as property address, rent price, number of bedrooms/bathrooms, description, contact info, and more.
* Save the extracted data in a clean, well-organized Excel file (`.xlsx` format).
* Support for pagination to scrape multiple pages of listings.

## Requirements

* Python 3.7 or above
* Libraries:

  * `requests` or `httpx`
  * `BeautifulSoup` (`bs4`)
  * `pandas`
  * `openpyxl`

You can install the dependencies using:

```bash
pip install requests beautifulsoup4 pandas openpyxl
```

## Usage

1. Clone the repository:

   ```git clone https://github.com/manojkumar2125/getRentsForRentFaster.ca.git
   
   ```

2. Run the scraper script:

   ```bash
   python scrape_rentfaster.py
   ```

3. After completion, check the generated Excel file `calgary_rentals.xlsx` in the project folder. The file will contain all the rental listings with details in separate columns.

## Output Excel Columns

* Title / Property Name
* Address
* City
* Rent Price
* Bedrooms
* Bathrooms
* Square Footage (if available)
* Description
* Listing URL

## Notes

* Make sure you comply with RentFaster.ca's terms of service before scraping data.
* The scraper handles pagination, but you may want to set limits to avoid overloading the server.
* The script can be customized to scrape specific cities or filter listings by criteria.

## Troubleshooting

* If you encounter issues with missing data, the website layout may have changed. Inspect and update the parsing logic accordingly.
* Ensure you have a stable internet connection when running the scraper.

## License

This project is licensed under the Manojkumar License.

