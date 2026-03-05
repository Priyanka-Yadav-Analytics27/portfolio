<h1 align="center">Priyanka Yadav</h1>

<p align="center">
Business Analytics • Marketing Analytics • Data Visualization
</p>

<p align="center">
SQL | Tableau | Python | Business Intelligence
</p>

<p align="center">
<a href="mailto:Priyankayadav01238@gmail.com">📧 Email</a> |
<a href="https://www.linkedin.com/in/yadav27/">🔗 LinkedIn</a>
</p>

<p align="center">
Welcome to my analytics portfolio where I showcase projects focused on data-driven business insights.
</p>

<hr>

## About Me

I’m a Business Analytics graduate with experience analyzing business, marketing, and operational data using SQL, Tableau, and statistical analysis.

My projects focus on transforming raw data into insights that improve decision-making, from customer lifetime value analysis to market investment evaluation and marketing optimization.

I’m currently pursuing roles in Business Analytics and Marketing Analytics.

## Tools & Technologies

**Languages**
![SQL](https://img.shields.io/badge/SQL-E6D9FF?style=for-the-badge&logo=postgresql&logoColor=black)
![Python](https://img.shields.io/badge/Python-D6F5E3?style=for-the-badge&logo=python&logoColor=black)

**Visualization**
![Tableau](https://img.shields.io/badge/Tableau-FFE3C8?style=for-the-badge&logo=tableau&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-DFF5E1?style=for-the-badge&logo=microsoft-excel&logoColor=black)

**Analytics**
![Marketing Analytics](https://img.shields.io/badge/Marketing%20Analytics-FFD6E8?style=for-the-badge&logo=googleanalytics&logoColor=black)
![Business Analytics](https://img.shields.io/badge/Business%20Analytics-D6E8FF?style=for-the-badge&logo=databricks&logoColor=black)
![Data Visualization](https://img.shields.io/badge/Data%20Visualization-FFF0B3?style=for-the-badge&logo=chartdotjs&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-E3D7FF?style=for-the-badge&logo=databricks&logoColor=black)

---

## Featured Projects

## 🎬 Film Rental SQL + Tableau Analytics

### Problem
A film rental company wanted to understand which customers and film categories were driving revenue, and how rental demand differed across locations. The company had large transaction datasets (customers, rentals, payments, inventory), but lacked clear insights into customer lifetime value, category demand patterns, and revenue concentration.

### My Approach
I wrote SQL queries to integrate data from multiple relational tables including customers, rentals, payments, films, and inventory. Using these queries, I built Tableau dashboards to analyze:
* rental volume by film category
* revenue distribution across customers
* rental demand by store location
* customer lifetime value (CLV)

The analysis focused on identifying high-value customers and high-performing content categories.

### Example SQL Query – Customer Lifetime Value Analysis

This query calculates Customer Lifetime Value (CLV) by identifying the customers who generated the highest revenue through rentals.

```sql
SELECT 
    c.customer_id,
    CONCAT(c.first_name, ' ', c.last_name) AS customer_name,
    COUNT(r.rental_id) AS total_rentals,
    SUM(p.amount) AS total_spent
FROM customer c
JOIN rental r ON c.customer_id = r.customer_id
JOIN payment p ON r.rental_id = p.rental_id
GROUP BY c.customer_id, customer_name
ORDER BY total_spent DESC
LIMIT 10;
```

### Key Insights
• Sports and Animation categories generated the highest rental volume, representing a significant share of total transactions.
• Customer spending followed a highly skewed distribution, where a relatively small group of repeat customers generated a large portion of total revenue.
• Rental demand varied across store locations, indicating potential opportunities to optimize inventory allocation by location and category demand.

### Business Impact

These insights could help the company:
* prioritize high-demand film categories when purchasing inventory
* identify and retain high-value customers through loyalty programs
* improve inventory placement across stores based on regional demand patterns

### Tools
SQL | Tableau | Data Visualization

![Film Rental Dashboard](film_rental_dashboard.png)

🔎[View Full Project](Film_Rental_SQL_Tableau_Analytics.pdf)

### Tools
SQL | Tableau | Data Visualization

---

## 🏙 Real Estate Market Selection & Investment Optimization

### Problem
An investment firm was evaluating multiple cities for a new real estate development project. The challenge was to determine which market would deliver the highest long-term financial return while minimizing vacancy risk.

### My Approach
I performed a comparative market analysis using key real estate investment metrics including:
* Net Operating Income (NOI)
* vacancy rates
* operating expenses
* projected property value appreciation

Financial modeling was used to simulate expected cash flow and equity growth across different market scenarios.

### Key Insight
• New Hope demonstrated the strongest projected Net Operating Income, outperforming other markets in the analysis.
• Lower vacancy projections indicated more stable rental demand, reducing long-term revenue risk.
• The combination of higher NOI and stronger property appreciation created the highest projected equity growth among the evaluated markets.

### Business Impact

Based on the financial modeling, New Hope represented the most attractive investment opportunity, balancing income stability with long-term value growth.

![Market Performance](real_estate_analysis.png)

🔎[View Full Project](Real_Estate_Market_Selection_and_Investment_Optimization.pdf)

### Tools
Financial Modeling | Market Analysis | Python | Excel

---

## 🏗 Construction Cost Operations Analytics

### Problem
Construction companies face significant financial risk due to volatile material prices and supplier dependencies. The goal of this analysis was to identify which material categories were most affected by price fluctuations and where procurement strategies could reduce cost exposure.

### My Approach
I analyzed procurement and cost datasets to evaluate:
* price volatility across material categories
* supplier concentration risk
* cost trends over time

The analysis focused on identifying materials with the highest price instability.

### Key Insight
• A small subset of construction materials showed significant price volatility over time, making them major drivers of cost uncertainty.
• Certain materials also exhibited high supplier concentration, increasing the risk of supply disruptions and price spikes.
• Identifying these high-risk categories highlights opportunities to diversify suppliers or negotiate long-term procurement contracts.

### Business Impact

The analysis provides procurement teams with actionable insights to reduce cost volatility and improve budgeting accuracy for large construction projects.

![Construction Analytics](construction_analytics.png)

🔎[View Full Project](Construction_Cost_Operations_Analytics.pdf)

### Tools
Operations Analytics | Cost Analysis

---

## 🤖📈 AI Marketing Campaign Optimization Strategy

### Problem
Marketing teams often struggle to analyze campaign performance quickly enough to optimize budgets, targeting, and creative strategies in real time. Manual analysis of campaign data can delay decision-making and reduce marketing ROI.

### My Approach
I designed a conceptual AI-powered marketing analytics system that continuously monitors campaign data and recommends optimizations such as:
* reallocating budgets across campaigns
* identifying underperforming audience segments
* recommending A/B testing opportunities

The system integrates campaign performance metrics to support faster data-driven decision making.


### Key Insight
• Real-time campaign monitoring enables marketing teams to identify performance trends earlier and adjust strategy proactively.
• Automated optimization recommendations can help allocate budgets toward higher-performing channels and audience segments.
• AI-driven analysis reduces the time required for campaign evaluation, allowing teams to scale experimentation and improve overall marketing efficiency.

### Business Impact
An automated campaign optimization system can significantly improve marketing ROI by enabling faster, data-driven adjustments to campaign strategy.

![Marketing AI](marketing_ai_framework.png)

🔎[View Full Project](AI_Marketing_Campaign_Optimization_Strategy.pdf)

### Tools
Marketing Analytics | AI Strategy | Campaign Optimization

---

## 🌱 EcoGrantGenie — AI Grant Writing Assistant

### Problem
Nonprofit organizations spend significant time and resources preparing grant proposals, often with limited staff capacity. This slows down the funding process and reduces the number of grant opportunities organizations can pursue.

### My Approach
I developed the concept for EcoGrantGenie, an AI-powered grant writing assistant that:
* analyzes grant requirements
* generates structured proposal drafts
* assists with refining proposal narratives

The system uses natural language processing to streamline the proposal creation process.

### Key Insight
• Automating early stages of grant writing can significantly reduce preparation time for nonprofit organizations.
• AI-generated proposal drafts help organizations focus more on strategy, storytelling, and impact articulation.
• The system can increase the number of grant applications nonprofits can submit within limited resource constraints.

### Business Impact
EcoGrantGenie can help nonprofits secure funding more efficiently while reducing the operational burden of grant proposal development.

![EcoGrantGenie](ecograntgenie_ai.png)

🔎[View Full Project](EcoGrantGenie_AI_Grant_Writing_Assistant.pdf)

### Tools
AI Product Design | NLP | LLM Prompt Engineering

<br>
<br>
<hr>

<p align="center">
Built by Priyanka Yadav • Business & Marketing Analytics Portfolio
</p>

<p align="center">
© 2026
</p>
