# Web Scraping ETL Pipeline. Top 50 Films

## Overview
This project implements an end to end ETL pipeline using Python.  
It extracts movie ranking data from a public archived webpage, transforms raw HTML into structured tabular data, and loads the results into persistent storage for analysis.

The project demonstrates practical skills in web scraping, data transformation, and database loading.

## Data Source
The data is scraped from an archived snapshot of the  
“100 Most Highly Ranked Films” page on EverybodyWiki.

## Dataset Description
The final dataset contains the following fields.

- Average Rank  
- Film Title  
- Release Year  

## ETL Pipeline

### Extract
- Send an HTTP request to the archived webpage  
- Parse HTML content using BeautifulSoup  
- Identify the ranking table  
- Extract the top 50 ranked films  

### Transform
- Convert extracted values to appropriate data types  
- Structure records into a pandas DataFrame  
- Enforce consistent column naming  

### Load
- Export the cleaned dataset to a CSV file  
- Load the dataset into a SQLite database  
- Replace existing records on re run  

## Technologies Used
- Python  
- Requests  
- BeautifulSoup  
- Pandas  
- SQLite  

## Project Outputs
- `top_50_films.csv`  
- `Movies.db` with table `Top_50`  

## How to Run
1. Install required Python libraries  
2. Run the Python script  
3. Inspect the CSV file or query the SQLite database  

## Why This Project Matters
This project mirrors real world data engineering workflows.  
It shows how to collect unstructured web data, transform it into a clean dataset, and persist it for analysis or downstream modeling.

## Skills Demonstrated
- Web scraping and HTML parsing  
- Data cleaning and transformation  
- CSV and database loading  
- End to end ETL pipeline design  

