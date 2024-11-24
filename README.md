# Myntra Insighter

**Myntra Insighter** is a comprehensive review scraping and analysis tool designed to extract, analyze, and visualize product reviews from Myntra. This project consists of two main components:  
- Review scraping  
- Insightful data analysis using dashboards  

The extracted reviews are stored in **MongoDB** for easy retrieval and processing.

---

## Table of Contents  
1. [Overview](#overview)  
2. [Features](#features)  
3. [Installation](#installation)  
4. [Usage](#usage)  
5. [Technologies Used](#technologies-used)   

---

## Overview  

**Myntra Insighter** enables users to:  
- Scrape reviews from Myntra products.  
- Store the scraped reviews in MongoDB.  
- Generate insightful visualizations, such as charts and graphs, to provide an overview of product ratings and customer feedback.  

---

## Features  

1. **Review Scraping**: Automatically scrape reviews from Myntra for any product.  
2. **MongoDB Integration**: Store and retrieve scraped data in MongoDB.  
3. **Dashboard Visualization**: Generate dynamic charts and summaries, providing a detailed look at product ratings and review sentiments.  
4. **Automated Data Extraction**: Extract key details such as product price, rating, and user comments from the scraped reviews.  
5. **Analysis Dashboard**: Visualize:  
   - Average product ratings  
   - Rating distribution  
   - Positive and negative review insights  

---

## Installation  

To set up the project locally, follow these steps:  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/AravaChoudhary/Mantra_Insighter.git 

2.	Navigate to the project directory:
    ```bash  
    cd Myntra Insighter  

3.	Install the required dependencies:
    ```bash  
    pip install -r requirements.txt  

4.	Set up MongoDB to store review data.

5.	Run the application:
    ```bash
    streamlit run app.py  


## Usage

1.	Scraping Reviews:
	•	Enter the product name or category.
	•	Set the number of products to scrape.
	•	The tool will automatically scrape reviews from Myntra.

2.	Data Visualization:
	•	The dashboard provides graphical insights into the reviews, including:
	•	Price distribution
	•	Rating analysis
	•	Positive/negative review highlights


## Technologies Used

	•	Python: Main programming language used for scraping and analysis.
	•	Streamlit: Frontend framework for displaying the data insights dashboard.
	•	MongoDB: NoSQL database to store scraped review data.
	•	Selenium: Web scraping framework for navigating and extracting data from Myntra.
	•	Pandas & Matplotlib: For data manipulation and visualization.


Happy Scraping and Analyzing! 🎉