# Coffee Sales Analysis

![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

This analysis is mainly focused on analysing and finding pattern of a dataset of coffee sales around United States, United Kingdom, and Ireland from the year 2019 to 2022. The dataset includes detailed information about each order, such as the date, the types of coffee served, their sizes, quantities, prices, etc. This data was collected from <b>[here](https://github.com/mochen862/excel-project-coffee-sales/blob/019f1f41f236a4c66a34282a85095648de48de3b/coffeeOrdersProject.xlsx)</b>. By the end of this project, I hope to showcase my skills and proficiency in Excel or spreadsheet programs in general.

### Preview of The Final Product of This Project

![final_dashboard](/assets/DashboardPreview.png)

## Project Structure

    ├── assets             <- Source for this project.
        │
        ├── Coffee Sales Analysis.xlsx           <- Finished project file.
        │   
        ├── Dashboard Preview.png                <- Additional images for preview.
        │
        ├── coffeeOrders_RAW.xlsx                <- The raw data that has not been cleaned.
    ├── README.md          <- README for using this project.

  
--------

### Step-by-Step Analysis in Excel

1. **Data Familiarization:**
   - Conducted an initial review of the dataset to understand its structure and identify potential insights.

2. **Handling Missing Data:**
   - Identified missing data points and used `XLOOKUP` and `INDEX MATCH` functions to retrieve and populate the required information accurately.

3. **Populating Sales Column:**
   - Added a `Sales` column using a simple multiplication formula to calculate total sales.

4. **Expanding Abbreviations:**
   - Created new columns `Coffee Type Name` and `Roast Type Name` to replace abbreviations with full names. Used the `IF` function for this purpose:
     ```excel
     =IF(I2="Rob","Robusta",IF(I2="Exc","Excelsa",IF(I2="Ara","Arabica",IF(I2="Lib","Liberica",""))))
     ```
     
     ```excel
     =IF(J2="M","Medium",IF(J2="L","Light",IF(J2="D","Dark","")))
     ```

5. **Data Formatting:**
   - Changed the date format to a more readable form.
   - Updated the size format to include "kg".
   - Added currency symbols to the price and sales columns to enhance readability.

6. **Duplicate Check and Removal:**
   - Utilized the `Remove Duplicates` feature to ensure data integrity. No duplicates were found.

7. **Table Conversion:**
   - Converted the data range to an actual Excel table for better management and analysis.

8. **Pivot Table Creation:**
   - Generated pivot tables to summarize key metrics:
     - **Total Sales Over Time:** Tracked sales trends over the specified period.
     - **Sales by Country:** Analyzed sales distribution across different countries.
     - **Top Customers:** Identified the top customers based on sales volume.

9. **Adding Slicers:**
   - Enhanced pivot tables with slicers for interactive filtering:
     - **Roast Type Name**
     - **Loyalty Card**
     - **Size**

10. **Timeline Addition:**
   - Incorporated a timeline for the `Order Date` to enable easy temporal analysis of sales data.

11. **Dashboard Creation:**
    - Developed an interactive dashboard featuring:
      - Pivot tables
      - Slicers
      - Timeline
    - The dashboard allows for dynamic exploration and visualization of sales data insights.

---

### Conclusion

This analysis provides a comprehensive overview of the coffee sales data, highlighting key trends, customer behaviors, and geographical distribution of sales. The interactive dashboard facilitates easy exploration and presentation of the insights derived from the data. The project can easily be accessed by downloading the file <b>[here](https://github.com/Fahruni/Coffee-Sales-Analysis/blob/main/assets/Coffee%20Sales%20Analysis.xlsx)</b> in which you can personally interact with the dashboard.
