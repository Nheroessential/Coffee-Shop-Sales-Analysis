This guided project gives us access to a rich dataset that is ready for investigation, sourced by [Maven Analytics](https://mavenanalytics.io/data-playground?pageSize=10&search=coffee+shop+sales). One excel sheet with transaction records for Maven Roasters, a fictional coffee business with three locations in New York City-Astoria, Lower Manhattan, and Hell's Kitchen is included in the dataset. Together with product-level information, the dataset also contains the transaction date, timestamp, and location.  
After downloading the dataset, I performed the following steps which are:
1. Data Cleaning
2. Data Analysis
3. Data visualization

## Data Cleaning
I performed a first visual examination of the dataset to grasp its organization before delving deeply into data cleaning. I took note of the quantity of fields and their respective definitions. This initial perspective, which included 149,456 records overall, laid the groundwork for a methodical approach to data analysis. After that, I started cleaning, starting with the elimination of duplicates. I searched for duplicates in the Excel by going to the data tab and then the data tools, where I used the "Remove Duplicates" tool.

After that, I used the "Conditional Formatting" feature from the home tab -> Styles section to highlight the cells that contained errors. I chose "New Rules" to open a formatting dialog, then I selected "format only cells that contain" and chose "Blanks" from the dropdown list. I then formatted the cell to highlight it in red and clicked OK. To date, no errors have been found.

I then formatted the column labeled "unit_price." by converting it to two decimal places of currency ($dollar).

Additionally, I created a few new columns to aid in my study. I included the following columns:
+ Revenue column; Revenue=(price*quantity)
+ Month and Day of the week; from “transaction_date” column
+ Hour; from “transaction_time” column

With minimal cleaning required due to primarily clean records, the dataset is now ready for advanced analysis. In the following step of analysis, we plan to extract useful insights and draw significant conclusions.

## Data Analysis
In this stage of data analysis, I used pivot tables to generate some useful insights. I generated pivot tables using the new columns I introduced. I had a total of five pivot tables, showing the following insights:  
+ Revenue by month
+ Number of transactions by day of the week
+ Number of transactions by hour of the day
+ Number of transactions by product categories
+ Number of transactions and revenue by product type


From the pivot table, I created eye-catching charts and included slicers for easier navigation. As we approach the final step – visualization — we are ready to convey our findings in a visually appealing and easily accessible style. Prepare to see the power of data visualization come to life!
