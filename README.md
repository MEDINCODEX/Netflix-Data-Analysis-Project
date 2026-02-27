
# 🎬 Netflix Data Analysis Project

## 📌 Project Overview

This project analyzes the Netflix dataset to explore trends, content distribution, and platform growth over time.

The goal of this project is to:
- Clean and prepare raw data
- Perform Exploratory Data Analysis (EDA)
- Extract meaningful insights
- Prepare the dataset for Power BI visualization
- Build an interactive dashboard

---

## 🛠 Tools & Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Power BI

---

## 📂 Dataset Description

The dataset contains information about Netflix content including:

- show_id
- type (Movie / TV Show)
- title
- director
- cast
- country
- date_added
- release_year
- rating
- duration
- listed_in (genre)
- description

---

## 🧹 Data Cleaning Process

The following cleaning steps were applied:

### 1️⃣ Handling Missing Values
- Filled or removed null values where necessary
- Cleaned country and rating columns

### 2️⃣ Date Conversion
Converted `date_added` to datetime format:

```python
df['date_added'] = pd.to_datetime(df['date_added'], errors='coerce')

Extracted:

year_added

month_added

3️⃣ Duration Cleaning

Separated duration into:

duration_minutes (for Movies)

seasons (for TV Shows)

Converted values from string to numeric format.

4️⃣ Removed Duplicates

Checked and removed duplicate rows to ensure clean data.

📊 Exploratory Data Analysis (EDA)

Key questions explored:

How many Movies vs TV Shows?

Which countries produce the most content?

How has Netflix grown over time?

What are the most common ratings?

What genres are most frequent?

📈 Key Insights

Movies represent the majority of content.

Content growth increased significantly after 2015.

The United States produces the highest number of titles.

TV-MA is one of the most common ratings.

📊 Power BI Dashboard

The cleaned dataset was exported and used in Power BI to build an interactive dashboard including:

Total Titles KPI

Movies vs TV Shows Distribution

Content Added per Year

Top 10 Countries

Ratings Distribution

Global Content Map

🚀 Project Structure
Netflix-Analysis/
│
├── data/
│   └── netflix_cleaned.csv
│
├── notebooks/
│   └── netflix_analysis.ipynb
│
├── powerbi/
│   └── netflix_dashboard.pbix
│
└── README.md
🎯 Skills Demonstrated

Data Cleaning

Data Transformation

EDA (Exploratory Data Analysis)

Data Visualization

Dashboard Design

Business Insight Extraction

📌 Conclusion

This project demonstrates the full data analysis workflow:
Raw Data → Cleaning → EDA → Insights → Dashboard

It showcases the ability to transform raw datasets into actionable business insights.

👨‍💻 Author

Created by [Your Name]"# Netflix-Data-Analysis-Project" 
