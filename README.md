# 📊 Netflix Data Wrangling & Preprocessing  

This project demonstrates a **complete data wrangling pipeline** using the **Netflix Movies and TV Shows dataset**.  
It includes **data gathering, cleaning, transformation (1NF, 2NF, 3NF), categorical encoding, data integration, PCA for dimensionality reduction, and visualization**.  

---

## 📂 Dataset  
- Source: [Netflix Movies and TV Shows on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)  
- File: `netflix_titles.csv`  
- Description: Contains ~8,800 Netflix shows with fields like *title, director, cast, country, date_added, release_year, duration, listed_in (genres)*, etc.  

---

## 🛠️ Project Workflow  

1. **Data Gathering**  
   - Load dataset from CSV into Pandas.  

2. **Data Cleaning**  
   - Handle missing values (`director`, `title`, etc.).  
   - Remove duplicates.  
   - Standardize date formats (`date_added`).  

3. **Data Transformation**  
   - Normalize dataset into **1NF, 2NF, 3NF** (splitting `cast` and `listed_in`).  
   - Create **categorical encodings** for columns (`type`, `country`).  

4. **Data Integration**  
   - Merge normalized tables (e.g., shows + genres + cast).  

5. **Data Reduction (PCA)**  
   - Apply **Principal Component Analysis (PCA)** to reduce dimensionality.  

6. **Data Visualization**  
   - Top 10 content producing countries.  
   - Scatter plot of PCA results.  

---

## 📊 Visualizations  

### Top 10 Content Producing Countries  
*(Bar chart output from project)*  

### PCA Scatter Plot  
*(2D visualization of reduced dimensions)*  

---

## 💻 Tech Stack  
- **Python**  
- **Pandas, NumPy** → Data Wrangling  
- **Matplotlib, Seaborn** → Visualization  
- **scikit-learn** → PCA  

---

## ⚙️ Installation & Usage  

Clone this repo and install dependencies:

```bash
# Clone repo
git clone https://github.com/YourUsername/netflix-data-wrangling.git
cd netflix-data-wrangling

# Install requirements
pip install -r requirements.txt
```

Run the Jupyter Notebook:

```bash
jupyter notebook netflix_data_wrangling.ipynb
```

---

## 📌 Project Structure  

```
netflix-data-wrangling/
│── netflix_data_wrangling.ipynb   # Main notebook
│── netflix_titles.csv             # Dataset (optional, or download from Kaggle)
│── requirements.txt               # Dependencies
│── README.md                      # Project Documentation
```

---

## 📜 License  
This project is licensed under the **MIT License** – free to use and share.  
