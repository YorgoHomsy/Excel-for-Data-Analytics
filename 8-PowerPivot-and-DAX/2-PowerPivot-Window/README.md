# Power Pivot — Window

This section covers how I use **"Power Pivot Window"** to clean, transform, and prepare data before analysis.

---

I used Power Pivot to solve the question:

> “When are the most job postings during the week?”

Here’s what I did and learned:

---

## 1. Establishing the Connection

First, I loaded my queries and selected **“Only Create Connection”** and **“Add to Data Model”**.  
This allowed me to access all tables in Power Pivot without cluttering my Excel sheets.

📷 *Image 1: Establishing connection between the queries*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/8c60ba99ffda89b3943e8a4d9d9caad10f8d36e5/8-PowerPivot-and-DAX/2-PowerPivot-Window/establishing%20connection.png)

---

## 2. Exploring the Power Pivot Window

Inside **Power Pivot → Manage**, I worked with three main views:

- **Data View**: I checked my tables and column types, making sure dates and IDs were correct.  
- **Diagram View**: I created relationships by dragging columns from one table to another. This let me connect, for example, job IDs between job listings and salaries.  
- **Calculation Area**: I wrote DAX measures like median salary and counts, which I could reuse dynamically in PivotTables.

---

## 3. Creating Relationships

I connected my tables so Excel could understand how the data relates:


This allowed proper aggregation:

- Counting jobs per skill  
- Averaging salaries  
- Filtering by date  

---

## 4. Using PivotTables to Solve My Question

With the data model ready, I inserted a PivotTable from:


Then I set up:

- **Rows** → Day of the week (from job posted dates)  
- **Values** → Count of job postings  

This setup let me see exactly when the most jobs are posted during the week.

📷 *Image 2: PivotTable showing job postings per day*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/8c60ba99ffda89b3943e8a4d9d9caad10f8d36e5/8-PowerPivot-and-DAX/2-PowerPivot-Window/When%20are%20the%20most%20job%20posting%20during%20the%20week.png)

