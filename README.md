# pandas-challenge-1
Module 4 Challenge

# Using Pandas to manipulate the financials of a fictional e-commerce company

I dove into a dataset from a fictional e-commerce company, exploring and analyzing data to address real-world business questions. My mission involved identifying top customers, popular product categories, calculating profits, and more. By the end of this task, I had a practical understanding of data exploration, transformation, and analysis, which prepared me for more complex data scenarios in my future career.
Part 1: Explore the Data
First, I imported the data. 
Secondly, viewed the data. 
Third, I wrote queries in order to learn the top category for quantities sold and the top clients purchasing those consumables 
Part 2: Transform the Data
First, I created a new column called line_subtotal, populated by multiplying unit_price x quantity 
Secondly, I created new columns total_weight and shipping_price. I populated total_weight by multiplying unit_weight by quantity.  I then populated shipping_price by mulipyling total_weight by $7 for orders over 50 pounds or by $10 for orders under 50 pounds. 
Third, I created a line_price column and populated it by adding line_subtotal + shipping_price * 1.0925 for 9.25% sales tax
Fourth, I created a line_cost column and populated it by multiplying unit_cost * quantity + shipping_price
Fifth, I created a line_profit column and populated it by subtracting line_price - line_cost
Part 3: Confirm your work:
I was given 3 email receipts showing the total prices for 3 orders. I had to confirm that my calculations matched the receipts.  I ended up creating 3 new dataframes, using loc to populate each with the line_price for the 3 order_id's. Yes, the totals matched the receipts.   
Part 4: Summarize and Analyze
First, I created 5 new dataframes, using loc to populate the line_price for each of the top 5 client IDs.  
Secondly, I created a new DataFrame showing the totals for the top 5 clients, including total units purchased, total shipping price, total revenue, and total profit. 
Third, I created a new DataFrame to rename column headings from the previous DataFrame. I defined the money columns.  Next, I created a new function named currency_format_millions, to convert dollar amount to millions.  I applied that new function to only the money columns. Finally, I renamed the columns one last time to include the fact that dollar amounts were in millions. 
Fourth, and final step, I sorted the updated data by "Total Profit (millions)" form highest to lowest and assigned the sort to a new DataFrame.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [License](#license)
- [Credits](#credits)
- [Contact Information](#contact-information)
- [Additional Reading](#additional-reading)

## Installation

1. Ensure you have Python 3.10 or higher installed.
2. Clone this repository: `git clone https://github.com/steve-vierling/pandas-challenge-1.git`

## Usage

1. Launch jupyter notebook: 'jupyter notebook' 
2. Open file wholesale_data_analysis_starter_code.ipynb

## File Structure

The project follows the following structure:

Code language: Python (python)\
pandas-challenge-1/\
├──wholesale_data_analysis_starter_code.ipynb 
|--README.md   
└─ Resources
  -client_dataset.csv

## License
This project is licensed under Steve Vierling Programming, Ltd.

## Credits
Author Steve Vierling  
Tutor Deborah, of D.U. Tutoring, provided helpful insight in making this Pandas data manipulation functional  
Steve referenced https://realpython.com/ for this README.md template  
Steve also referenced all of the prior exercises inside the D.U. Artificial Intelligence course; https://bootcamp.du.edu/artificial-intelligence-062024/

## Contact Information
For any questions or feedback, feel free to message Steve at his linkedin site: https://www.linkedin.com/in/stephenvierling/

## Additional Reading 
See all of Steve's existing Python work here: https://github.com/steve-vierling 
I am a beginner python developer with a Master's degree in Information Systems from Regis University, Denver, CO. I have over 20 years of Unix/Linux experience, software support and 2.5 years in DevOps.  I am passionate about creating efficient and scalable software solutions.


