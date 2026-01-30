# DAX Advanced 

This section covers how I use **Advanced Transformation** to clean, transform, and prepare data before analysis.

---

## Solving: What's the Pay of the Top 10 Skills in the UK?

When I first tried to put `job_skills` in **Rows** and **median salary** in **Values**, I ran into a problem:  

> The default one-way relationships in Power Pivot blocked proper filtering between tables.

I learned that to fix this, I could:

- Use **cross-filtering** (`CROSSFILTER`) to allow both tables to filter each other  
- Create a **measure** in the skills table that calculates the **median salary** while respecting this relationship  

This let me drop `job_skills` in **Rows** and see their corresponding **median salary**, giving a clear view of the **top-paying skills**.

📸 *Image 1: What's the pay of the top 10 skills in the UK for Data Analyst*

![image alt](https://github.com/YorgoHomsy/Excel-for-Data-Analytics/blob/d509043b69914ee901d4c1e30b180d9e0c8c136d/8-PowerPivot-and-DAX/4-Dax-Advanced/What's%20the%20pay%20of%20the%20top%2010%20skills%20in%20the%20UK.png)

---

## Calculating Likelihood

I also explored **likelihoods**, which help answer:

> “How likely is a skill to lead to above-median pay?”

I learned to calculate it as:
Likelihood = (number of jobs with the skill paying above median) ÷ (total jobs with the skill)


Using this approach, I could see that some skills, like **Excel**, are not only in demand but also more likely to lead to **higher pay in the UK**.

