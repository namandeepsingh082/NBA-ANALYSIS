### 📊 **NBA Salary Analysis Using BigQuery & Looker Studio**  

🚀 **Tech Stack:**  
- **Google BigQuery** – Data storage & SQL analysis  
- **Looker Studio** – Interactive visualizations  
- **LookML** – Data modeling (if applicable)  
- **Google Cloud Platform (GCP)** – Cloud-based data processing  

## 🔍 **Project Overview**  
This project analyzes **NBA player salaries** based on **position, age, and team expenditures**, providing insights through **BigQuery SQL queries and Looker Studio dashboards**.  

### 🏀 **Key Insights**  
✅ **Position-based salary distribution** (Pie chart)  
✅ **Average player age by position** (Pie chart)  
✅ **Top 8 highest-paid players** (Bar chart)  
✅ **Top 8 highest-spending teams** (Bar chart)  

## 📈 **Visualizations**  

### 🎯 **Position-Based Salary Breakdown**  
- A **pie chart** categorizing players' salaries based on their **positions**.  
- Helps in understanding which positions are the highest-paid.  

### 🎯 **Average Age by Position**  
- Another **pie chart** showing the **average age** of players in each position.  
- Useful for analyzing player longevity in different roles.  

### 🎯 **Top 8 Highest-Paid Players**  
- A **bar chart** displaying **player names vs. salaries**.  
- Identifies the **highest-paid** players in the NBA.  

### 🎯 **Top 8 Teams by Salary Expenditure**  
- A **bar chart** ranking **teams** based on **total player salaries**.  
- Helps compare spending strategies across teams.  


## 🔍 **SQL Queries Used**  

### 1️⃣ **Position-Based Salary Distribution**  
```sql
SELECT position, SUM(salary) AS total_salary
FROM nba_data
GROUP BY position
ORDER BY total_salary DESC;
```

### 2️⃣ **Average Age by Position**  
```sql
SELECT position, AVG(age) AS avg_age
FROM nba_data
GROUP BY position;
```

### 3️⃣ **Top 8 Highest-Paid Players**  
```sql
SELECT player_name, salary
FROM nba_data
ORDER BY salary DESC
LIMIT 8;
```

### 4️⃣ **Top 8 Teams by Salary**  
```sql
SELECT team_name, SUM(salary) AS total_salary
FROM nba_data
GROUP BY team_name
ORDER BY total_salary DESC
LIMIT 8;
```

## 🚀 **How to Use This Project?**  
1️⃣ **Dataset:** Load NBA salary data into **Google BigQuery**.  
2️⃣ **SQL Analysis:** Run the provided queries to extract insights.  
3️⃣ **Visualization:** Use **Looker Studio** to create the charts & dashboards.  
4️⃣ **Presentation:** Share insights through interactive dashboards.  

## 📌 **Live Dashboard & Code**  
🔗 **[Looker Studio Dashboard](https://lookerstudio.google.com/reporting/5a58f08a-01fd-49bf-bf64-84fc8b520ca2)**  
🔗 **[GitHub Repository](https://github.com/namandeepsingh082/NBA-ANALYSIS)**  
![Screenshot 2025-03-08 043859](https://github.com/user-attachments/assets/e09c1be2-8924-4429-90d3-f3421551e671)

## 🛠 **Future Enhancements**  
✅ Add **trend analysis** for salary growth over the years.  
✅ Integrate **player performance metrics** (e.g., points per game).  
✅ Use **LookML models** for advanced data exploration.  
