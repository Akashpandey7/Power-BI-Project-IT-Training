# Power-BI-Project-IT-Training

The project is about creating a real-time end-to-end sales report with different visuals to best show sales insights in a one-page dashboard. The project involves gathering requirements, collecting data from multiple sources, implementing data modeling, performing additional data cleaning, creating unique keys, and generating reports with calculations such as revenue and profit.


1. ***Data Gathering / Requirement:***

- Collect the necessary data files for sales, categories, geography, product, salesrep, and subcategories.
- Load all the files from the sales folder into a single sales fact table using a mechanism that is resilient to missing files and automatically adds new yearly sales files.
- Create different visuals to best show sales insights in a one-page dashboard.



2. ***Data Modeling:***

- Transform the sales fact table to split the country from the city in the Location field and set up the correct data type to allow Geo maps.
- Update the Date field to ensure correct date format.
- Create a unique key (GeoKey) in the Sales and Geography tables.
- Create a small function to clean up the ID columns in SalesRep and Sub Category queries.
- Create the data model connecting all tables using the calendar table already set up in the pbix.

![DATA Modeling](https://user-images.githubusercontent.com/128131674/227862913-c3005bf6-a65e-4957-9ca6-5a5f4828a673.PNG)


3. ***DAX Calculations:***

- Calculate Total Revenue in the Sales table by using the Product's Retail Price and multiplying it by the Units.
- Calculate Total Cost in the Sales table by using the Product's Standard Cost and multiplying it by the Units.
- Calculate Gross Profit in Sales by subtracting Total Cost from Total Revenue.
- Calculate Gross profit MoM growth Change% measure.
- Calculate AVG sales per day measure.
- Calculate QoQ Growth.

![QoQ Growth](https://user-images.githubusercontent.com/128131674/227863920-7adad478-4283-4e1c-813d-91de05163394.PNG)


4. ***Sales Reports and Dashboard:***

- Use the calculated measures and visualizations to assemble a sales report with different visuals.
- Ensure the months are sorted from Jan-Dec if you plot Month on the x-axis.

