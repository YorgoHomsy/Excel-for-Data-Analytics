# Power Pivot — Introduction

This section covers how I use **"Power Pivot intro"** to clean, transform, and prepare data before analysis.

---

## Power Pivot — Introduction

In this section, I moved beyond single-table analysis and learned how Power Pivot turns Excel into a real data-modeling tool.

I worked with data loaded from Power Query into the Data Model, which allowed me to analyze multiple tables together instead of flattening everything into one sheet. Inside **Power Pivot → Manage**, I explored how data is stored, connected, and calculated at a deeper level.

One key thing I learned is why **DAX** is necessary. Standard PivotTables don’t support everything (like median), so I created custom measures in Power Pivot to calculate values dynamically based on filters and context. This made the analysis far more flexible and accurate.

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/452f2d4a8e1da7fff42275b89a47537026804f6f/8-PowerPivot-and-DAX/1-PowerPivot-Intro/creating%20dax%20formula%20median.png)

I also learned how to build and understand **relationships between tables** using the **Diagram View**. Seeing the **1 → many** structure visually helped me understand how filters flow and why some PivotTable setups work while others trigger relationship warnings.

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/452f2d4a8e1da7fff42275b89a47537026804f6f/8-PowerPivot-and-DAX/1-PowerPivot-Intro/View%20of%20the%20power%20pivot%20manage%20button.png)

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/452f2d4a8e1da7fff42275b89a47537026804f6f/8-PowerPivot-and-DAX/1-PowerPivot-Intro/Diagram%20View%20.png)

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/452f2d4a8e1da7fff42275b89a47537026804f6f/8-PowerPivot-and-DAX/1-PowerPivot-Intro/establishing%20a%20connection.png)




Finally, I tested everything by building PivotTables from the Data Model, which made it clear how:

- rows define the question  
- values must come from a table that can answer it  
- and why relationship direction actually matters  

---

Overall, this part showed me how **Power Pivot connects Power Query, DAX, and PivotTables into one coherent analytical workflow** — and why it’s essential for serious Excel analysis.
