# 🫁 Lung Capacity Analysis Project

A data analysis and visualization project that investigates the relationship between lung capacity and various categorical and numerical features. This project uses Python's data science libraries to provide insights into how factors such as gender, smoking status, age, height, etc., affect an individual's lung capacity.

---

## 📌 Objective

The primary objective of this project is to:
- Explore and understand the dataset.
- Perform correlation analysis between numeric features.
- Visualize the relationship between categorical variables and lung capacity.
- Derive meaningful insights using visual analytics.

---

## 📂 Project Files

| File | Description |
|------|-------------|
| `LungCap_project.ipynb` | Main Jupyter notebook with data preprocessing, correlation analysis, and visualizations. |
| `README.md` | Documentation for understanding and running the project. |
| *(Optional)* `LungCap.csv` | Dataset file used for analysis (not included in this repo unless uploaded). |

---

## 🧪 Techniques Used

- **Data Cleaning & Exploration**
  - Handling missing values
  - Separating categorical and numeric columns

- **Correlation Analysis**
  - Using `.corr(numeric_only=True)` to examine relationships among numeric variables
  - Heatmap visualization to represent the correlation matrix

- **Visualization**
  - Loop-based barplot generation for each categorical column:
    ```python
    for col in obj.columns:
        plt.figure()
        sns.barplot(x=col, y='LungCap', data=df, ci='sd')
    ```
  - Heatmaps, barplots, and other plots using `seaborn` and `matplotlib`

---

## 📊 Sample Visualizations

- ✅ **Correlation Heatmap**  
  Highlights the strength and direction of relationships between numerical columns.

- ✅ **Bar Plots for Categorical Columns**  
  Visually compares average lung capacity across groups like Gender, Smoke status, etc., using error bars (standard deviation).

- ✅ **Customizable Plot Appearance**  
  Easily extendable to include additional styling like hue, palette, layout, and saving to file.

---

## 📦 Libraries Required

Ensure you have the following Python libraries installed:

```bash
pip install pandas numpy matplotlib seaborn notebook
