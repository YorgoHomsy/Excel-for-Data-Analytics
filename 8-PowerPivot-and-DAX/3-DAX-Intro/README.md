# DAX — Introduction

This section shows how I used DAX inside Excel’s Data Model to answer real questions from the data, not just calculate numbers.

---

## What I was trying to answer

I started with a simple question: **what patterns can we discover in job postings and pay?**

That led me to explore:
- When jobs are posted  
- How skills relate to salary  
- How pay changes by country  

All of this was driven by **DAX measures**, not static calculations.

---

## 1. Aggregation — turning raw data into signals

I used DAX to **count jobs**, **count skills**, and **compare them properly**.  
A key learning here was understanding the difference between:

- **Distinct values** → how many different jobs exist  
- **Total rows** → how many skill entries exist  

This step let me calculate things like **average skills per job** in a reliable way, without breaking the model or hard-coding logic.

📸 *Image 1: using aggregation measures inside the Data Model*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/922a518ed0913a4911e8ceb8903cb844fe125642/8-PowerPivot-and-DAX/3-DAX-Intro/Aggregation.png)
---

## 2. Statistics — skills vs pay

Next, I moved beyond simple counts and looked at **median salary**, which gives a more realistic picture than averages.

By plotting **skills per job vs median salary**, I could clearly see the trend:

- Jobs that require more skills generally pay more  
- Engineers often need more skills than analysts, yet their median salaries can be surprisingly similar  

This is where DAX really clicked for me — **measures reacting dynamically to the data** instead of static calculations.

📸 *Image 2: skills per job vs median salary (scatter result)*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/922a518ed0913a4911e8ceb8903cb844fe125642/8-PowerPivot-and-DAX/3-DAX-Intro/statistics%20graph%20result.png)

---

## 3. Filters — comparing countries properly

Then I used DAX to compare **US vs non-US salaries**, and later drilled into specific countries.

This made it easy to:

- Lock the US median salary as a reference  
- Compare it directly with other countries using slicers  
- See how the same role behaves differently depending on location  


📸 *Image 3: UK median salary vs US*  

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/922a518ed0913a4911e8ceb8903cb844fe125642/8-PowerPivot-and-DAX/3-DAX-Intro/Comparing%20median.png)

📸 *Image 4: Australia vs US and non-US comparison*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/922a518ed0913a4911e8ceb8903cb844fe125642/8-PowerPivot-and-DAX/3-DAX-Intro/Comparing%20Australia%20to%20US%20and%20Non%20US.png)

One interesting outcome:
- Australia and the UK can outperform the US for certain roles, even when global medians are lower.
---

## Why this matters

Through this project, I learned how DAX:

- Turns raw tables into **business questions**
- Responds instantly to **filters and slicers**
- Makes Excel behave more like a **real analytics tool**

This wasn’t about memorizing formulas — it was about **thinking analytically** and letting the **data model do the heavy lifting**.
