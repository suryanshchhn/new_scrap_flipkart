# new_scrap_flipkart
Product Review Scraper

This is a web scraping application built with Flask, designed to scrape product reviews from Flipkart. The scraped reviews are then stored in a MongoDB database. The application provides a REST API endpoint to perform the scraping process.

Features:
-->Scrapes product reviews from Flipkart based on search queries.
-->Stores the scraped reviews in a MongoDB database.
-->Provides a REST API endpoint for easy integration with other applications.

Technologies Used:
-->Flask: Python web framework for building the application.
-->BeautifulSoup: Python library for parsing HTML content.
-->MongoDB: NoSQL database for storing the scraped reviews.
-->REST API: Allows other applications to interact with the scraper.

Setup and Usage:
1)Clone the repository to your local machine:
-->  git clone https://github.com/your-username/your-repo.git

2)Install the required dependencies:
-->  pip install -r requirements.txt

3)Make sure you have MongoDB installed and running on your machine. Update the MongoDB connection string in the code to point to your MongoDB database.

4)Run the Flask application:
-->  python app.py
The application will be running on port 5001. If you want to change the port, you can modify the app.run() line in the app.py file accordingly.

5)Access the application in your browser at http://localhost:5001/ or use the provided REST API endpoint to send requests for scraping reviews.

REST API Endpoint:
-->Endpoint: /review
-->Method: POST
-->Parameters:
-->content: The search query for the product reviews.

Example usage with cURL:
-->  curl -X POST -d "content=iphone" http://localhost:5001/review


INPUT PAGE
![INPUTPAGE](https://github.com/suryanshchhn/new_scrap_flipkart/assets/123889322/226e82d0-58a9-4749-aee5-55c01188a1de)

RESULT PAGE
![RESULTPAGE](https://github.com/suryanshchhn/new_scrap_flipkart/assets/123889322/8a7e767f-9991-4a9e-8f6e-343d59df099b)


