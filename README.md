# 📊 Netflix Power BI Dashboard Project

This project explores and visualizes Netflix's global content library using Power BI. The dataset contains thousands of titles, including movies and TV shows, along with information like ratings, directors, release years, and countries of origin.

## 🗂 Dataset Source

The dataset used is [Netflix Titles Dataset](https://www.kaggle.com/shivamb/netflix-shows), originally sourced from Kaggle. It was uploaded and transformed within Power BI for analysis.

## 🛠 Tools & Technologies

- **Power BI**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**
- **Data Transformation & Modeling**
- **Data Visualization**

## 🧩 Data Cleaning & Transformation

1. **Data Import**: Loaded the Netflix dataset CSV into Power BI.
2. **Power Query Editor**:
   - Checked and corrected data types for all columns.
   - Created two new columns:
     - `Country_new`: Extracted and cleaned country names.
     - `Director_new`: Extracted and cleaned director names.
   - Removed any null or unnecessary values.
3. **Applied & Loaded** the transformed data to the Power BI data model.

## 🧮 DAX Measures Created

```DAX
Movies = CALCULATE(DISTINCTCOUNT(netflix_titles[show_id]), FILTER(netflix_titles, netflix_titles[type]= "Movie"))

TV Show = CALCULATE(DISTINCTCOUNT(netflix_titles[show_id]), FILTER(netflix_titles, netflix_titles[type]= "TV Show"))

Total show = CALCULATE(DISTINCTCOUNT(netflix_titles[show_id]))

Total Director = CALCULATE(DISTINCTCOUNT(netflix_titles[Director_new]))
```

## 📈 Dashboard Features

- **Total Shows by Type (Pie Chart)**: Comparison between Movies and TV Shows.  
- **Total Shows by Release Year (Line Graph)**: Shows the growth trend of Netflix content over time, especially post-2010.  
- **Total Shows by Rating (Bar Chart)**: Highlights the popularity and diversity of content ratings, with TV-MA being the most frequent.  
- **Type of Show by Director (Donut Chart)**: Distribution of show types by director.  
- **Total Shows by Country (Map)**: A global view of content production distribution.

---

## 💡 Insights Derived

- Over **69%** of Netflix content consists of movies; TV shows make up the remaining **30%**.  
- A noticeable spike in content release was observed post-2015, indicating Netflix's rapid content expansion.  
- The **United States** and **India** are among the top content-producing countries on the platform.  
- Content rated **TV-MA** dominates, reflecting mature themes in Netflix programming.

---

## 🧠 Skills Demonstrated

- Data Cleaning and Transformation in Power Query  
- Creating Custom DAX Measures  
- Data Storytelling and Visual Design  
- Problem-Solving with Real-World Data  
- Dashboard Development with Interactivity and Filters  

---

## 🔗 Project Link

You can view the dashboard screenshots and download the `.pbix` file from the **[GitHub Repository](#)**  
> _(Update this with your actual GitHub repository link)_

