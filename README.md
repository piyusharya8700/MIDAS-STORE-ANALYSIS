# Midas Store Sales Analysis (2022)

![Midas Store Dashboard](/Screenshot%202026-05-31%20234623.png)

## What is this project?
I built this interactive Excel dashboard to analyze a year's worth of sales and order data for Midas Store. The goal was simple: take a messy, raw dataset of e-commerce transactions and turn it into clear, actionable business insights that show exactly who is buying, where sales are coming from, and how the business is growing.

---

## What the data tells us
* **Our biggest buyers:** Women are driving the business, making up **64%** of total sales, with adult women being our largest individual customer segment.
* **Top States:** **Maharashtra** is our biggest market by far, followed by Karnataka and Uttar Pradesh.
* **Where people shop:** **Amazon** is the clear favorite, bringing in **35%** of all orders, while Myntra and Flipkart run a close second and third.
* **Order Health:** The store is running smoothly with a **92% delivery success rate**. Cancellations and returns are incredibly low (around 2-3% each).
* **Seasonality:** March was our absolute peak month for both total order count and revenue before sales stabilized for the rest of the year.

---

## How I cleaned and processed the data
Before building any charts, I spent time cleaning up the raw data inside Excel to make sure the metrics were 100% accurate:
1. **Standardized Genders:** Cleaned up inconsistencies in the data where text entries were mixed (like fixing "W" to "Women" and "M" to "Men").
2. **Fixed Order Quantities:** Found and fixed typos in the quantity column where numbers were typed out as text (e.g., changing "One" to `1`) so calculations wouldn't break.
3. **Created Custom Buckets:** Extracted the text month from the order dates and used conditional logic to group customer ages into clean categories (*Teenager, Adult, Senior Citizen*) for better tracking.

---

## 🔬 Advanced Data Extraction & Formula Auditing
To complement the visual dashboard, I built out an analytical test bench within the workbook to practice industry-standard corporate data queries commonly required in MIS Executive and Business Analyst environments.

### Core Logic Practiced:
* **Dynamic Index Searches:** Implementing `XLOOKUP` arrays to bypass standard column positioning limits and extract targeted transactional rows instantly.
* **Multi-Criteria Segmentation:** Using `COUNTIFS` to isolate specific intersecting customer demographics (e.g., matching marital status attributes with precise household family constraints).
* **Financial Aggregation Tracking:** Writing `SUMIFS` formulas to aggregate large-scale numerical columns against strict categorical strings while maintaining absolute range alignment.
* **Nested Logical Audits:** Combining `IF` conditional statements with embedded lookups to parse back-end variables and return custom, human-readable operational compliance tags.

### 📊 Formula Verification Reference
Below is the verified test sheet logging the implementation and execution of these advanced lookup and logical formulas:

![Formula Practice Log](Screenshot%202026-06-17%20204923.png)

*The live, interactive formulas tracking these evaluations can be inspected directly inside the [MIDAS STORE ANALYSIS.xlsx](./MIDAS%20STORE%20ANALYSIS.xlsx) workbook.*

---

## Dashboard Features
The final file includes a fully interactive sheet equipped with:
* **Dynamic Slicers:** You can filter the entire dashboard instantly by **State**, **Clothing Size**, or **Product Category**.
* **Dual-Axis Performance Chart:** Tracks total revenue (bars) alongside total order volume (line) over 12 months.
* **Breakdown Visuals:** Clear distribution charts for gender splits, age demographics, and sales channel shares.

---

## Tools I Used
* **Microsoft Excel:** Advanced Pivot Tables, Excel Formulas & Functions (Data Cleaning, XLOOKUP, SUMIFS, Nested Logic), Data Validation, and UI/Dashboard Design.

---

## How to test it out
1. Download the `MIDAS STORE ANALYSIS.xlsx` file from this repository.
2. Open it up in Microsoft Excel.
3. Check out the formula test bench tab to see advanced lookup and aggregation statements in action!
4. Use the slicer buttons on the right side of the dashboard to filter through different regions and product sizes!
