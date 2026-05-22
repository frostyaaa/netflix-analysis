# netflix-analysis
Netflix data cleaning and analysis

# 📺 Netflix Data Analysis Using Python

This project performs Exploratory Data Analysis (EDA) on the Netflix dataset using Python and visualization libraries to uncover business insights and content trends.

## 📌 Project Objective

The main objective of this project is to clean, analyze, and visualize Netflix data to answer important business questions such as:

- Which content type dominates Netflix?
- Which countries produce the most Netflix content?
- Which genres are most common?
- Who are Netflix's top content creators?
- How has Netflix content changed over time?
- Which ratings dominate the platform?

---

## 📂 Dataset Information

The dataset contains information about Netflix titles including:

- Show ID
- Type (Movie / TV Show)
- Title
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genre
- Description

---

## 🧹 Data Cleaning Process

The following preprocessing steps were performed:

✔ Removed unnecessary columns (`Unnamed: 0`, duplicate fields)

✔ Converted `date_added` to datetime format

```python
df["date_added"] = pd.to_datetime(
    df["date_added"],
    errors="coerce"
)
```

✔ Split duration into:

- `duration_value`
- `duration_type`

Example:

| Original | Duration Value | Duration Type |
|-----------|----------------|---------------|
| 90 min | 90 | min |
| 3 Seasons | 3 | Seasons |

✔ Handled missing values

✔ Standardized text values

✔ Split and cleaned multi-value columns

---

## 📊 Business Questions Solved

### 1. Which content type dominates Netflix?

- Movie vs TV Show distribution

### 2. Which countries produce the highest Netflix content?

- Top content-producing countries

### 3. How has Netflix content grown over time?

- Year-wise trend analysis

### 4. Which ratings are most common?

- Audience target analysis

### 5. Which genres dominate Netflix?

- Most popular genres

### 6. Who are Netflix's top content creators?

- Top directors on Netflix

### 7. What month sees maximum content additions?

- Monthly content trends

### 8. Movie duration distribution

- Runtime analysis

### 9. TV show season distribution

- Season count analysis

### 10. Which actors appear most frequently?

- Top recurring actors

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📈 Visualization Examples

Project includes:

- Count Plots
- Horizontal Bar Charts
- Histograms
- Line Charts
- Boxplots
- Distribution Plots

---

## 🚀 How to Run

Clone this repository:

```bash
git clone <repository-link>
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```bash
Netflix_Analysis.ipynb
```

---

## 📌 Key Insights

- Movies dominate Netflix content.
- Certain countries contribute significantly more content.
- Drama and international content appear frequently.
- Netflix focuses heavily on mature audience categories.
- Content production has increased rapidly over recent years.

---

## 📷 Project Preview

(Add screenshots of visualizations here)

Example:

![Dashboard](images/dashboard.png)

---

## 👨‍💻 Author

Devraj

GitHub: https://github.com/frostyaaa

LinkedIn: https://linkedin.com/in/devraj0807

---

⭐ If you found this project useful, consider giving it a star.
