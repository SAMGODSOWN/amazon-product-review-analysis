[![Project Status]
# Amazon Product Review Analysis (Excel)

## 📁 Project Files
- **Data**: [sample_data.xlsx](data/sample_data.xlsx)  
- **Template**: [analysis_template.xlsx](templates/analysis_template.xlsx)  
- **Report**: [project_report.pdf](docs/project_report.pdf)  

## 📊 Key Features
- Exports visualizations for trends, ratings, and keyword frequency.  
- Uses Power Query for automated data cleaning.  
[My DSA Amazon Project Real (1).xlsx](https://github.com/user-attachments/files/21088783/My.DSA.Amazon.Project.Real.1.xlsx)
![AMAZON PRO JECT REAL 3](https://github.com/user-attachments/assets/9c64a199-8d62-4026-9fcf-7e89487f5173)
![AMAZON PRO JECT REAL 1](https://github.com/user-attachments/assets/e390710b-d881-4be6-87aa-2798379d668d)
![AMAZON PRO JECT REAL 2](https://github.com/user-attachments/assets/65a7920c-bceb-40bc-9e92-62a0b9f38020)
![AMAZON PRO JECT REAL 6PNG](https://github.com/user-attachments/assets/a20320f7-f958-4e68-b689-8f4c7b87b41d)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Analyzes Amazon product review data using Excel (Power Query, PivotTables, and sentiment scoring). Exports visualizations for trends, ratings, and keyword frequency.
This project is a deep dive into Amazon product reviews, discounts, and pricing, showcasing my foundational analytical skills developed during the DSA Incubator program. Through the strategic application of Excel's powerful features like pivot tables, slicers, and calculated fields, I've transformed raw e-commerce data into **actionable insights** aimed at guiding product enhancements, refining marketing strategies, and boosting customer engagement.

## Table of Contents
- [🔍 Project Overview](#project-overview)
- [📊 Dataset Insights](#dataset-insights)
- [📋 Core Analytical Questions & Approaches](#core-analytical-questions--approaches)
- [📈 Key Business Discoveries & Impact](#key-business-discoveries--impact)
- [🛠️ Technologies Utilized](#technologies-utilized)
- [🚀 Project Structure](#project-structure)
- [📸 Visuals & Dashboard Snapshot](#visuals--dashboard-snapshot)
- [⭐ My Analytical Toolkit in Action](#my-analytical-toolkit-in-action)
- [📬 Connect with Me](#connect-with-me)

## 🔍 Project Overview

As a **Beginner Data Analyst**, this project served as a hands-on learning experience to extract valuable intelligence from Amazon product and customer review data. My primary goal was to illuminate key trends and patterns that could empower e-commerce stakeholders to make more informed decisions, ultimately fostering **data-driven improvements** in product offerings and customer satisfaction.

## 📊 Dataset Insights

My analysis was conducted on a publicly available dataset meticulously scraped from Amazon product pages. This comprehensive collection encompasses **1,465 unique product records**, detailed across **16 distinct columns**.

**Highlights of the Data Fields:**
- `Product Name` and `Category`
- `Actual Price` & `Discounted Price`
- `Discount %` (a crucial calculated metric)
- `Rating` (average product satisfaction score)
- `Rating Count` (total volume of customer feedback)
- Aggregated `Review Content`
- Derived metrics like `Potential Revenue` to gauge market opportunity.

## 📋 Core Analytical Questions & Approaches

To derive meaningful insights, I tackled a series of business-centric questions, employing various Excel functionalities:

| # | Analytical Question                                                 | Excel Approach & Logic Used                                      |
|---|---------------------------------------------------------------------|------------------------------------------------------------------|
| 1 | What is the average discount percentage by product category?        | Pivot Table with AVERAGE function                                |
| 2 | How many products are listed under each category?                   | Pivot Table using COUNT of unique products                       |
| 3 | What is the total number of reviews per category?                   | Pivot Table with SUM of `Rating Count`                           |
| 4 | Which products boast the highest average ratings?                   | Data Sorting + Pivot Table displaying Average `Rating`           |
| 5 | What is the average actual price vs. discounted price by category?  | Pivot Table comparing Averages of `Actual Price` and `Discounted Price` |
| 6 | Which products have accumulated the highest number of reviews?      | Data Sorting + Pivot Table with SUM of `Rating Count`            |
| 7 | How many products feature a discount of 50% or more?                | Filtering Logic and COUNTROWS function                           |
| 8 | What is the distribution pattern of product ratings (e.g., 3.0, 4.0)? | Pivot Table with Product Counts grouped by `Rating`              |
| 9 | What is the total potential revenue (`actual_price` × `rating_count`) per category? | Creation of a Calculated Column + Pivot Table with SUM of `Potential Revenue` |
| 10| What is the unique product count per defined price range bucket (<₹200, ₹200–₹500, >₹500)? | `IF` formulas for custom bucketing + Pivot Table (COUNT unique) |
| 11| How does product rating relate to the level of discount offered?    | Grouping Discounts + Pivot Table showing Average `Rating`        |
| 12| How many products currently have fewer than 1,000 reviews?          | Filtering Logic and COUNTROWS function                           |
| 13| Which categories feature products with the highest average discounts? | Sorted Pivot Table by AVERAGE `Discount %` per category          |
| 14| Identifying the top 5 products based on combined review count and rating. | Custom Ranking Logic (e.g., a weighted score combining both metrics) |

## 📈 Key Business Discoveries & Impact

My analysis yielded several significant insights, offering valuable perspectives for e-commerce strategies:

* **Optimizing Revenue Streams:** Discovered that categories like **Home & Kitchen** and **Electronics** hold the highest `Potential Revenue`. This insight is crucial for prioritizing marketing spend and inventory focus on products with strong market demand and customer engagement.
* **Smarter Pricing Strategies:** Revealed that a **high discount doesn't automatically translate to higher product ratings or customer satisfaction**. This finding empowers sellers to move beyond aggressive discounting and explore more sustainable pricing models while maintaining positive customer perception.
* **Boosting Customer Engagement:** Identified **Electronics and Accessories** as leading categories in customer reviews. This suggests prime opportunities for implementing targeted feedback campaigns, community building, or loyalty programs to deepen customer relationships.
* **Strategic Product Development:** Highlighted products with solid review volumes but moderate ratings. These represent excellent opportunities for **focused quality improvements** or targeted feedback collection, allowing for a strategic uplift in customer satisfaction.
* **Informed Market Positioning:** Gained clarity on product distribution across various price points. This understanding is vital for **competitive analysis** and making data-backed decisions on pricing, new product introductions, and market segmentation.

## 🛠️ Technologies Utilized

This project was developed primarily using **Microsoft Excel**, demonstrating proficiency in:

* **Data Transformation & Analysis:**
    * Pivot Tables and Pivot Charts
    * Calculated Columns and Fields
    * Advanced Excel Formulas (`IF`, `COUNTIF`, `AVERAGEIFS`, `SUMIFS`, `PROPER`)
    * Data Grouping and Filtering
* **Data Visualization & Reporting:**
    * Interactive Dashboards
    * Slicers and Timelines
    * Conditional Formatting
    * Various Chart Types (Bar, Line, Donut, Cards)
* **Data Handling:**
    * Named Ranges & Table References
* **Data Source:** Web-scraped Amazon product review data

## 🚀 Project Structure

This GitHub repository is structured to provide a clear overview and access to all project components:

* `Amazon Product Review Analysis.xlsx`: The core Excel workbook, containing the raw data, cleaned datasets, all analytical pivot tables, calculated fields, and the interactive dashboard.
* `screenshots/`: A dedicated folder housing high-quality images that showcase key dashboard views and charts.
* `README.md`: This comprehensive document, serving as the project's executive summary and guide.

## 📸 Visuals & Dashboard Snapshot

Below are snapshots from the interactive dashboard, providing a glimpse into the generated insights:

![AMAZON PRO JECT REAL 3](https://github.com/user-attachments/assets/9c64a199-8d62-4026-9fcf-7e89487f5173)
*A sample table view, display  cleaned dataset.*

![AMAZON PRO JECT REAL 1](https://github.com/user-attachments/assets/e390710b-d881-4be6-87aa-2798379d668d)
*A pivot table showing and exploring between product discount percentages and average customer ratings and others.*

![AMAZON PRO JECT REAL 2](https://github.com/user-attachments/assets/65a7920c-bceb-40bc-9e92-62a0b9f38020)
*A pivot table illustrating the total calculated potential revenue across various product categories and others.*

![AMAZON PRO JECT REAL 6PNG](https://github.com/user-attachments/assets/a20320f7-f958-4e68-b689-8f4c7b87b41d)
*A comprehensive view of the interactive dashboard, showcasing key performance indicators,category trends and others.*

⭐ My Analytical Toolkit in Action: Foundations & Growth
This project serves as a clear demonstration of my growing analytical capabilities and the foundational skills I'm actively building. It highlights my practical application of core data analysis principles to real-world challenges:
 * Data Structuring & Aggregation: I effectively leveraged Excel's pivot tables to summarize complex datasets, showcasing my ability to transform raw data into digestible formats. This involved applying calculated columns and various formulas for essential data cleaning, transformations, and generating new metrics that provided deeper insights.
 * Building Interactive Visualizations: I successfully designed and implemented a dynamic and intuitive Excel dashboard. By integrating diverse visual elements and interactive slicers, I learned to transform complex data into clear, compelling narratives, empowering user-driven exploration of product performance.
 * Translating Data into Actionable Insights: A key focus for me was learning to articulate data findings into clear, actionable recommendations. This involved developing my ability to discern patterns, identify opportunities, and frame insights within the context of business challenges, directly informing potential product strategies and customer experiences.
 * Structured Problem-Solving: I approached a diverse set of 14 analytical questions systematically. This hands-on experience, from understanding pricing impacts to customer sentiment, reinforced my structured and thorough approach to data-driven problem-solving, even as a beginner.
 * Ensuring Data Quality: I prioritized data integrity by implementing diligent cleaning practices, including handling null values and ensuring consistent data formats. This commitment to data quality is a crucial step in ensuring the accuracy and reliability of all analytical outputs.*

📬 Connect with Me
I'm continuously learning and excited to connect with fellow data enthusiasts and professionals. Please feel free to reach out for questions, feedback on my work, or potential collaborations as I continue my journey in data analytics!
[![Name]]
   Obadire Samuel Abimbola 
[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail)](mailto:samuelobadire176@gmail.com)  
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin)](https://linkedin.com/in/obadire-usefuls)  
[![Phone](https://img.shields.io/badge/-Phone-25D366?logo=whatsapp)](tel:+2348025363954)  
