This guided project gives us access to a rich dataset that is ready for investigation, sourced by [Maven Analytics](https://mavenanalytics.io/data-playground?pageSize=10&search=coffee+shop+sales). One excel sheet with transaction records for Maven Roasters, a fictional coffee business with three locations in New York City-Astoria, Lower Manhattan, and Hell's Kitchen is included in the dataset. Together with product-level information, the dataset also contains the transaction date, timestamp, and location.  

![Coffee raw](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/7a11d0ed-26ba-43c9-8aee-e7710ffa5dae)

After downloading the dataset, I performed the following steps which are:
1. Data Cleaning
2. Data Analysis
3. Data visualization

## Data Cleaning
I performed a first visual examination of the dataset to grasp its organization before delving deeply into data cleaning. I took note of the quantity of fields and their respective definitions. This initial perspective, which included 149,456 records overall, laid the groundwork for a methodical approach to data analysis. After that, I started cleaning, starting with the elimination of duplicates. I searched for duplicates in the Excel by going to the data tab and then the data tools, where I used the "Remove Duplicates" tool.

![Remove duplicates](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/085b7536-ea90-4278-b44b-d61def580930)

After that, I used the "Conditional Formatting" feature from the home tab -> Styles section to highlight the cells that contained errors. I chose "New Rules" to open a formatting dialog, then I selected "format only cells that contain" and chose "Blanks" from the dropdown list. I then formatted the cell to highlight it in red and clicked OK. To date, no errors have been found.

![Conditional formatting](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/77519443-dc5f-45ba-8f47-8322ef626375)

I then formatted the column labeled "unit_price." by converting it to two decimal places of currency ($dollar).

![Currency formatting](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/a549063f-dc73-4af6-b709-2beb11881a55)

Additionally, I created a few new columns to aid in my study. I included the following columns:
+ Revenue column; Revenue=(price*quantity)
+ Month and Day of the week; from “transaction_date” column
+ Hour; from “transaction_time” column

![Added Columns](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/724db9fa-be91-4b81-9d15-a8a0b8def3a6)

With minimal cleaning required due to primarily clean records, the dataset is now ready for advanced analysis. In the following step of analysis, we plan to extract useful insights and draw significant conclusions.

## Data Analysis
In this stage of data analysis, I used pivot tables to generate some useful insights. I generated pivot tables using the new columns I introduced. I had a total of five pivot tables, showing the following insights:  
+ Revenue by month
+ Number of transactions by day of the week
+ Number of transactions by hour of the day
+ Number of transactions by product categories
+ Number of transactions and revenue by product type

![pivottable](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/4b798f78-0b84-4eb7-8516-a51489104bcc)


From the pivot table, I created eye-catching charts and included slicers for easier navigation. As we approach the final step – visualization — we are ready to convey our findings in a visually appealing and easily accessible style. Prepare to see the power of data visualization come to life!

![Dashboard](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/fcd73e4e-22b9-40b5-934b-b7d50f4ccbcc)

From here, it is easy to analyze a location at a time using the slicer.

Sales in Astoria peak on Mondays, Wednesdays, Thursdays, and Fridays. The busiest hours are from 7:00 to 10:00 a.m., with consistency between 11:00 and 19:00 p.m.
![Astoria](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/f7ffc86f-8448-467a-84ec-f6eac2ba7d90)

The busiest days for transactions in Hell's Kitchen are Tuesdays, Fridays, and Sundays. Sales are highest between 8:00 and 10:00 a.m., and drop dramatically between 19:00 and 20:00 p.m.
![HK](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/795e413d-81ef-4e5e-b489-6a852998459d)

Mondays are busiest days in Lower Manhattan, while the rest of the week is rather consistent. Sales are highest between 7:00 to 10:00, with a dip in the late evening from 19:00 to 20:00.
![LW](https://github.com/Nheroessential/Coffee-Shop-Sales-Analysis/assets/90351195/1f5eecbc-c46d-4c83-a6db-50d6b64b2b86)

The overall revenue per month began at $80,000 in January, dropped slightly in February, and then progressively grew from March to June, ranging from $100,000 to $180,000.

Transactions by day of week in the area show that Monday, Wednesday, Thursday, and Friday have the highest sales, while Tuesday, Saturday, and Sunday have stable sales.

Transactions by hour of the day show a considerable increase in the early hours, while sales decline in the evening, with fewer products sold.

Transactions by product category show that coffee, tea, and pastry items are the best-selling. Among the top 15 goods across all locations, Barista Espresso has the most income, while Sugar-Free Syrup has the lowest.

### Recommendations
To improve operational efficiency and revenue, consider altering operating hours, especially during sluggish periods. According to the data, sales drop dramatically between 19:00 and 20:00. As a result, starting operations at 6:00 a.m. and ending at 18:00 p.m. appears to be a viable option. This change coincides with customer demand patterns, ensuring that resources are utilized efficiently during peak hours while reducing unnecessary expenses associated with extended evening operations.

Implementing a proactive approach to inventory management and production scheduling to ensure that coffee, tea, and pastry items are appropriately stocked during business hours. By regularly monitoring sales patterns and modifying production levels as needed, we can ensure a consistent supply of these popular items to fulfill consumer expectations.


