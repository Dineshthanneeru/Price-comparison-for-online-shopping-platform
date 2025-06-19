# **Price Comparison Tool for Online Shopping (Python Web Scraping)**

## **Overview**

This tool allows users to compare prices and ratings for a product across multiple Indian e-commerce websites, namely Amazon and Flipkart. It uses Python and web scraping techniques to fetch real-time data directly from product search pages. The tool is aimed at helping users make smarter purchase decisions by presenting prices side-by-side in a command-line interface.

## **Features**

- Lightweight and easy to run from terminal

- Scrapes price and rating data from Amazon and Flipkart

- Automatically formats and compares product listings

- Simple logic and minimal dependencies

- Gracefully handles missing data or unexpected website structure

## **Updates**

- Removed hard dependencies on non-standard libraries

- Basic error handling is included (more verbose errors can be added)

- Works on modern Python versions (tested on Python 3.12)

- Can be easily extended to more platforms like Croma, Reliance Digital, etc.

- Optimized selectors for higher accuracy with current site structure

## **Motivation**

With so many e-commerce platforms offering the same product at varying prices, it's time-consuming to manually search and compare deals. This script automates that process, saving both time and effort. While it started as a personal utility, it has evolved into a shareable tool to help others compare prices more effectively and learn basic web scraping along the way.

## **Installation**

To run the program locally:
```
git clone https://github.com/your-username/price-comparison-tool.git
cd price-comparison-tool
pip install -r requirements.txt
```
Note: You may want to run this in a Python virtual environment to avoid dependency conflicts.

## **Usage**
```
python price_comparison.py
```
You'll be prompted to enter a product name (e.g., Samsung Galaxy M14). The tool will fetch and display the price and rating for that product from both Amazon and Flipkart.

## **Sample Output:**
```
Enter the product name: Samsung Galaxy M14

Price and Rating Comparison:
Amazon: Price - ₹12,999, Rating - 4.3 out of 5 stars
Flipkart: Price - ₹12,499, Rating - 4.4
```
## **Requirements**

- Python 3.7+

- Internet connection (to fetch live data)

- The following Python libraries:
    - requests
    - beautifulsoup4

To install dependencies:

```
pip install requests beautifulsoup4
```

## **Known Issues**

- Site structure may change over time, breaking the scraper (requires updates to class names or parsing logic)

- Amazon and Flipkart may block repeated requests or show CAPTCHA for suspicious activity

- No use of user-agent or header spoofing (can be added for stability)

## **Future Work**

- Add support for more websites (e.g., TataCliq, Croma, Reliance Digital)

- Export comparison results to a CSV or Excel file

- Add GUI using Tkinter or Streamlit

- Introduce proper logging and error reporting

- Handle CAPTCHA / blocked requests using Selenium or proxy rotation

## **Disclaimer**

This is an educational project meant for learning and experimentation. Web scraping may violate the terms of service of some websites. Please use this script responsibly and ethically. The author is not responsible for any misuse.

## **Contributing**

Contributions are welcome! If you find bugs or want to extend this tool with more features, feel free to fork the repo and submit a pull request. For major changes, please open an issue first to discuss the proposal.
