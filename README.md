# Airbnb_data_analysis
# Airbnb Data Analysis: Chicago vs New Orleans

This repository contains a Power BI project that analyzes Airbnb listings data for Chicago and New Orleans. The data is sourced from [Inside Airbnb](https://insideairbnb.com/get-the-data/), and it addresses real-world challenges such as market trends, pricing analysis, and financial evaluation similar to an industry-standard Airbnb dashboard.

## Table of Contents

- [Dataset Overview](#dataset-overview)
- [Data Transformation Methodology](#data-transformation-methodology)
- [Dashboard Features & Real-World Insights](#dashboard-features--real-world-insights)
- [How to Run](#how-to-run)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

## Dataset Overview

The project utilizes datasets available on [Inside Airbnb](https://insideairbnb.com/get-the-data/), which include detailed information about Airbnb listings such as:

- Listing details (price, room type, and location)
- Host information
- Availability calendars
- Review scores and dates

This rich dataset provides the foundation for a comprehensive comparative analysis of Airbnb markets in Chicago and New Orleans.

## Data Transformation Methodology

Data transformation is performed in Power BI using **Power Query**. Below is a step-by-step outline of the process:

### 1. Importing the Data
- **Download and Import:**  
  Download the CSV or JSON files for Chicago and New Orleans and import them into Power BI as separate queries.
- **Initial Loading:**  
  Verify that each dataset loads correctly in the Power Query Editor.

### 2. Data Cleaning and Formatting
- **Filtering & Removing Unnecessary Columns:**  
  Remove columns that are not essential for your analysis (e.g., internal IDs, redundant descriptions).
- **Handling Null Values & Duplicates:**  
  - Use column filters to identify and filter out rows with null values in critical fields.
  - Remove duplicate records by using the "Remove Duplicates" option or grouping rows by unique identifiers.
- **Type Conversion:**  
  Ensure date and numeric columns are correctly formatted. Use **Change Type > Using Locale** if needed (for instance, MM/DD/YYYY vs DD/MM/YYYY).

### 3. Creating Custom Columns
- **City Identification:**  
  Add a custom column in each query to tag the data with the appropriate city name (e.g., "Chicago" and "New Orleans"). This is used when appending the datasets.
- **Additional Metrics:**  
  Create calculated columns (e.g., occupancy rate, average review score) for further analysis.

### 4. Data Standardization and Appending
- **Standardize Column Names:**  
  Ensure column names match exactly between the two datasets to facilitate a smooth append.
- **Appending the Data:**  
  Append the cleaned datasets together into a single unified query, and verify that the "City" column reflects the correct labels.
- **Final Validation:**  
  Check for any errors or inconsistencies by sampling rows and validating data types before clicking **Close & Apply**.

## Dashboard Features & Real-World Insights

The final Power BI dashboard is designed to provide interactive, actionable insights, including:

### City Comparison Features
- **Interactive Visuals:**  
  - **Comparison Charts:**  
    Visualizations such as clustered bar charts display key metrics (e.g., average price, number of listings, review scores) side-by-side for Chicago and New Orleans.
  - **Map Visualizations:**  
    Geographic maps pinpoint listing locations, highlighting neighborhood-level insights.
- **Dynamic Filtering:**  
  - **Slicers:**  
    Allow users to filter by city, room type, or price range.
  - **Drill-Downs:**  
    Enable deeper exploration by drilling down into specific neighborhoods or time periods.
- **Consistent Layout:**  
  Consistent color-coding, legends, and themes are used for clear and direct comparisons between the two cities.

### Real-World Insights
- **Market Trends Analysis:**  
  Examine seasonal fluctuations, pricing strategies, and availability trends to inform investment decisions.
- **Customer Behavior:**  
  Analyze review patterns and host responsiveness to gauge customer satisfaction.
- **Financial Insights:**  
  Evaluate potential revenue by comparing average nightly prices and occupancy rates, offering a financial perspective akin to industry case studies.
- **Strategic Decision-Making:**  
  Provide stakeholders with a robust tool for understanding market dynamics and making data-driven decisions.

## How to Run

1. **Download the Repository:**  
   Clone or download this repository to your local machine.
2. **Open the Power BI File:**  
   Open the `Airbnb_viz.pbix` file in Power BI Desktop.
3. **Explore the Data Transformation:**  
   Review the steps in the Power Query Editor to understand how the data was cleaned, standardized, and appended.
4. **Interact with the Dashboard:**  
   Navigate through the report pages, use slicers and filters to explore detailed insights for Chicago and New Orleans.

## Future Work

- **Additional Visualizations:**  
  Integrate more granular data analyses, such as time-series forecasting or sentiment analysis from review data.
- **Live Data Connections:**  
  Explore connecting directly to live data sources for real-time updates.
- **Advanced Financial Metrics:**  
  Incorporate deeper financial analysis tools to enhance revenue forecasting.

## Acknowledgments

Thanks to [Inside Airbnb](https://insideairbnb.com/get-the-data/) for providing comprehensive datasets and to Labmentix Edtech Pvt. Ltd. for support during this project.

## Contact

For any questions or suggestions, please open an issue or contact me directly.

---

This README outlines the comprehensive work involved in transforming raw Airbnb datasets into an interactive analytical dashboard, showcasing how real-world problems—like market analysis and financial case studies—can be solved using Power BI.
