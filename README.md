# Adventure Works Sales & Budget Performance Dashboard

## Project Overview

This project delivers an interactive Power BI dashboard designed for the sales team at Adventure Works. The primary goal is to provide comprehensive insights into sales performance, customer behavior, and product analytics, enabling data-driven decision-making. The dashboard aims to answer key business questions related to sales trends, budget adherence, geographical performance, and detailed product/customer insights.

## Features & Deliverables

The dashboard was developed following best practices in Power BI and includes the following key features:

1.  **Data Cleaning & Transformation (Power Query):**
    * Performed extensive data cleaning, shaping, and transformation using Power Query Editor.
    * Ensured data quality, consistency, and optimized data types for efficient analysis.

2.  **Robust Data Model:**
    * Designed a star schema data model with fact tables (e.g., Sales, Budget) and dimension tables (e.g., Calendar, Products, Customers, Territory, Product Category, Product Subcategory).
    * Established strong relationships between tables to enable seamless data filtering and aggregation.

3.  **Calculated Columns & Measures (DAX):**
    * Created essential calculated columns using DAX to enhance the data model (e.g., DateKey in Calendar table for time intelligence).
    * Developed a comprehensive set of DAX measures for key performance indicators (KPIs) and analytical calculations, including:
        * `Total Sales`
        * `Total Budget`
        * `Gross Profit`
        * `Total Order Quantity`
        * `Sales vs. Budget` (Absolute difference)
        * `Sales vs. Budget %` (Percentage difference)
        * And other relevant measures for detailed analysis.

4.  **Diverse Visualizations:**
    * Utilized a wide range of Power BI's native visuals to present data effectively:
        * **KPI Cards:** For high-level summaries of `Total Sales`, `Total Budget`, `Gross Profit`, and `Sales vs. Budget %`.
        * **Line Charts:** To visualize sales trends over time.
        * **Bar/Column Charts:** For comparing sales across product categories, customer segments, and top N products.
        * **Donut Charts:** To show proportional breakdowns (e.g., Sales by Customer Segments).
        * **Map Visuals:** To display sales performance across different geographical regions/countries.

5.  **Interactive Filters & Slicers:**
    * Implemented multiple slicers (e.g., Date, Product Category, Sales Territory Group, Product Color, Customer Occupation, Yearly Income) for dynamic filtering and exploration of data.
    * Ensured slicers are synchronized across relevant pages for a cohesive user experience.

6.  **Multi-Page Dashboard Layout:**
    * The dashboard consists of at least two dedicated pages to provide both a high-level overview and detailed insights:
        * **Page 1: Sales Overview & Performance:** Focuses on overall sales trends, budget adherence, and geographical distribution.
        * **Page 2: Product & Customer Deep Dive:** Provides granular analysis of product performance and customer demographics.

7.  **Enhanced User Experience (Tooltips, Buttons & Bookmarks):**
    * **Custom Tooltips:** Configured tooltips for key visuals to provide additional context and detailed information on hover.
    * **Navigation Buttons:** Implemented buttons for seamless navigation between the "Sales Overview" and "Product & Customer Details" pages.
    * **Bookmarks:** Created and integrated a "Clear All Filters" bookmark with a dedicated button to reset all slicers and return the dashboard to its default view.

8.  **Row-Level Security (RLS):**
    * Implemented RLS to control data access based on user roles.
    * Defined roles (e.g., `North America Manager`, `Europe Manager`, `Pacific Manager`) with specific data filtering rules based on the `Territory[Group]` column.
    * Enabled secure viewing of data, ensuring users only see the information relevant to their assigned region.

9.  **Aesthetic Design & Theming:**
    * Applied a consistent and visually appealing color theme throughout the dashboard for improved readability and user engagement.
    * Ensured proper alignment, consistent font usage, and optimized spacing for a professional look.
    * Implemented conditional formatting for the `Sales vs. Budget %` KPI to visually highlight performance (e.g., green for positive, red for negative).

## Getting Started

To view and interact with the dashboard:

1.  **Download:** Clone this repository or download the `Adventure Works Sales & Budget Performance.pbix` file.
2.  **Open:** Open the `.pbix` file using Power BI Desktop.
3.  **Explore:** Navigate through the different pages, use the slicers, and interact with the visuals to gain insights.
4.  **(Optional) Test RLS:** In Power BI Desktop, go to the "Modeling" tab -> "View as roles" and select a defined role (e.g., `North America Manager`) to see how RLS restricts data visibility.

## Data Source

The dashboard utilizes sales, budget, and dimension data derived from the Adventure Works sample database, provided as .xlsx file within this repository.

## Contribution

This project was developed as part of a Power BI training program. For any questions or feedback, please open an issue in this repository.

---
