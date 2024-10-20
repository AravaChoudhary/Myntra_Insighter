# Mantra_Insighter

Mantra_Insighter is a comprehensive review scraping and analysis tool specifically designed to extract, analyze, and visualize product reviews from Myntra. The project consists of two main components: review scraping and insightful data analysis using dashboards. The extracted reviews are stored in MongoDB for easy retrieval and processing.
Table of Contents

# Overview
Features
Installation
Usage
Dashboard Generation Process
ScrapeReviews Code Flow
Technologies Used
Contributing
Overview

Mantra_Insighter enables users to:
Scrape reviews from Myntra products.
Store the scraped reviews in MongoDB.
Generate insightful visualizations, such as charts and graphs, to provide an overview of product ratings and customer feedback.
Features

Review Scraping: Automatically scrape reviews from Myntra for any product.
MongoDB Integration: Store and retrieve scraped data in MongoDB.
Dashboard Visualization: Generate dynamic charts and summaries, providing a detailed look at product ratings and review sentiments.
Automated Data Extraction: Extract key details such as product price, rating, and user comments from the scraped reviews.
Analysis Dashboard: Visualize:
Average product ratings
Rating distribution
Positive and negative review insights
Installation

To set up the project locally:
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/Mantra_Insighter.git
Navigate to the project directory:
bash
Copy code
cd Mantra_Insighter
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Set up MongoDB to store review data.
Run the application:
bash
Copy code
streamlit run app.py
Usage

Scraping Reviews: Enter the product name or category, set the number of products, and the tool will automatically scrape reviews from Myntra.
Data Visualization: The dashboard provides graphical insights into the reviews, including price distribution, rating analysis, and positive/negative review highlights.
Dashboard Generation Process

The DashboardGenerator class is responsible for generating detailed visual summaries of the scraped reviews. Below is an overview of the process flow:
__init__: Initializes the dashboard with the review data.
display_general_info(): Converts product ratings and prices to numeric and generates pie and bar charts to summarize average ratings and prices by product.
display_product_sections(): Displays product sections, including:
Average price and rating
Top positive reviews (rating ≥ 4.5)
Top negative reviews (rating ≤ 2)
Rating distribution (by count)
ScrapeReviews Code Flow

The ScrapeReviews class automates the review scraping process, utilizing Selenium to interact with the product pages. Below is the flow for scraping reviews:
__init__: Initializes the Chrome driver and sets the product name and number of products to scrape.
scrape_product_urls(): Converts the product name to a search query, retrieves product URLs, and returns the list of URLs.
extract_reviews(product_link): Extracts review titles, ratings, prices, and links to detailed reviews from the product page.
scroll_to_load_reviews(): Scrolls through the page to load more reviews dynamically.
extract_products(product_reviews): Extracts user ratings, comments, usernames, and stores them in a DataFrame.
get_review_data(): Compiles all review data into a DataFrame and saves it to a CSV file.
Technologies Used

Python: Main programming language used for scraping and analysis.
Streamlit: Frontend framework for displaying the data insights dashboard.
MongoDB: NoSQL database to store scraped review data.
Selenium: Web scraping framework for navigating and extracting data from Myntra.
Pandas & Matplotlib: For data manipulation and visualization.
Contributing

Contributions are welcome! If you'd like to contribute to Mantra_Insighter, please fork the repository and make a pull request with your changes.