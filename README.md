# Mars Data Scraping and Analysis

## Overview

This project involves web scraping and data analysis focused on Mars news and weather data. The goal is to extract relevant information from a Mars news site and a Mars weather dataset, analyze the data, and visualize key insights.

## Part 1: Scraping Mars News Data

### Steps:

1. **Automated Browsing with Splinter**
   - Use Splinter to navigate to the Mars news site.
   - Extract the HTML content of the page.

2. **Extracting Titles and Preview Text**
   - Use Beautiful Soup to parse the HTML content.
   - Locate and extract the titles and preview text of news articles.

3. **Storing Data**
   - Store the extracted information in a list of dictionaries. Each dictionary contains:
     ```python
     {"title": "Article Title", "preview": "Article Preview"}
     ```

## Part 2: Scraping and Analyzing Mars Weather Data

### Steps:

1. **Extract HTML Table into Pandas DataFrame**
   - Use Pandas or a combination of Beautiful Soup and Pandas to parse the HTML table into a DataFrame.
   - Ensure columns are correctly named and data types are properly set.

2. **Data Analysis**

   - **Number of Months on Mars**
     - Determine the number of unique months in the dataset.

   - **Number of Martian Days**
     - Calculate the total number of Martian days based on the dataset.

   - **Temperature Analysis**
     - Compute the average temperature for each month.
     - Identify the months with the lowest and highest average temperatures.
     - Visualize this data using a bar chart.

   - **Atmospheric Pressure Analysis**
     - Compute the average atmospheric pressure for each month.
     - Identify the months with the lowest and highest average atmospheric pressures.
     - Visualize this data using a bar chart.

   - **Martian Year Length**
     - Estimate the number of terrestrial days in a Martian year.
     - Provide a visual estimate within 25%.

3. **Export DataFrame to CSV**
   - Save the DataFrame to a CSV file using:
     ```python
     DataFrame.to_csv('filename.csv')
     ```

## Technologies Used

- **Splinter**: For automated browsing.
- **Beautiful Soup**: For HTML parsing.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib/Seaborn**: For data visualization.

## Installation

To run this project, ensure you have the required libraries installed. You can install them using pip:

```bash
pip install splinter beautifulsoup4 pandas matplotlib seaborn
