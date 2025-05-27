# EDA Car Prices

## Project Overview
This project explores the factors that influence used car prices through exploratory data analysis. Using a comprehensive dataset of over 558,000 used car sales records from Kaggle, I analyzed various vehicle attributes and their relationship with selling price.

## Dataset
The dataset contains detailed information about used car sales from a major automotive marketplace, including:
- Vehicle details (make, model, year, body type, transmission)
- Sale information (price, MMR value, condition)
- Other attributes (odometer reading, color, interior, state)

The Kaggle dataset includes 558,837 records with 16 columns, providing a rich source for analysis of the used car market dynamics. you can find the dataset here: https://www.kaggle.com/code/khaledsayedaaaaa/eda-car-price/input

## Analysis Approach
The analysis follows a structured approach:

1. **Data Cleaning & Preprocessing**
   - Handling missing values and duplicates through careful examination
   - Standardizing categorical variables like make and body types through extensive string manipulation
   - Converting datetime information from string format to proper datetime objects
   - Normalizing text fields for consistent analysis
   - Filtering extreme price values to focus on typical market transactions
   - Extensive work on standardizing the body column to ensure consistent brand representation:
        - >First converted all body types to lowercase, then used regex patterns to standardize similar terms - like combining all types of 'cab' into 'Truck'. This cleaned up over 50 messy categories into just 7 clear body types.
           ![image](https://github.com/user-attachments/assets/b3ec1373-9eed-45f1-a1ad-6cacc8b7bf21)

     


2. **Feature Engineering**
   - Creating a price_deviation column to measure the difference between MMR (Manheim Market Report) value and actual selling price
   - Removing outliers based on price deviation to focus on typical market behavior
   - Calculating car age based on sale date and manufacturing year

3. **Exploratory Analysis**
   - Correlation Analysis and measuring the relationship between numerical variables
   - Analyzing price distribution across different vehicle makes and models
   - Examining the relationship between vehicle condition and selling price
   - Investigating how odometer readings impact vehicle valuation
   - Exploring the correlation between vehicle age and price depreciation
   - Assessing how body type and transmission affect pricing
   - Evaluating the impact of color and interior options on vehicle value
   - Identifying geographical pricing variations across different states

5. **Visualization**
   - Creating informative histograms for the distribution of the data and plots to illustrate key findings
   - Using correlation matrices to display relationships between variables
   - bar charts and histograms to show price distributions
  
     > Here's a scatter plot showing car mileage vs price. Each dot represents a car, with colors indicating its condition. The plot reveals that higher mileage cars generally sell for less money, with better condition cars (shown in greener colors) typically commanding higher prices.
     ![image](https://github.com/user-attachments/assets/4996e369-3095-4971-8fab-665aa266a6b9)


## Tools & Technologies
- Python
- Pandas for data manipulation
- Matplotlib/Seaborn for visualization
- Jupyter Notebook for analysis environment

*This project was completed as part of a data analysis showcasing skills in exploratory data analysis and data visualization.* 
