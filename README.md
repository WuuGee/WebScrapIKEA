# IKEA Malaysia Product Scraper

A Python automation script built with Selenium and Pandas that scrapes product details from the [IKEA Malaysia](https://www.ikea.com/my/en/) website. The script reads a list of product names from a CSV file, navigates through search results (handling Swedish character normalization), and extracts detailed specifications—including handling different color variations of the same product.

## 🚀 Features

* **Automated Search:** Iterates through a list of products automatically.
* **Color Variation Handling:** Detects if a product has multiple colors, visits each variation, and extracts the specific details for that color.
* **Data Extraction:** Scrapes the following fields:
    * Product Name
    * Color
    * Price
    * Article Number (SKU)
    * Summary
    * Dimensions
* **Swedish Character Normalization:** Automatically converts characters like `Ä`, `Ö`, `Å` to standard English characters to ensure accurate search matching.
* **Excel Export:** Appends data to an Excel file (`StoreProduct.xlsx`) in real-time, ensuring data is saved even if the script stops unexpectedly.

## 🛠️ Prerequisites

Before running this script, ensure you have the following installed:

* [Python 3.x](https://www.python.org/downloads/)
* [Google Chrome](https://www.google.com/chrome/)
* [ChromeDriver](https://chromedriver.chromium.org/downloads) (Ensure the version matches your installed Chrome browser)

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/WuuGee/WebScrapIKEA.git
   cd WebScrapIKEA

2. **Install the required Python libraries:**
   ```bash
   pip install selenium pandas beautifulsoup4 requests openpyxl

## ⚙️ Configuration & Usage

1. **Prepare the Input File**
   Create a file named ProductName.csv in the root directory.
   The first row should be a header (e.g., Product Name).
   List the products you want to scrape in the first column.

   **Example `ProductName.csv`:**
    ```csv
    Product Name
    BILLY
    MALM
    KALLAX
    POÄNG

2. **Run the Script**
   ```bash
   pip install selenium pandas beautifulsoup4 requests openpyxl
