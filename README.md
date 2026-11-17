# ♻️ Plastic Waste and Recycling Analytics

## 📌 Project Overview

This project focuses on analyzing plastic waste generation, recycling performance, and waste management practices across different cities in India.

Using Python and data visualization libraries, the project explores waste generation patterns, recycling rates, disposal methods, and management costs to identify meaningful insights and understand the effectiveness of plastic waste management.

## 🎯 Project Objectives

- Analyze plastic waste generation across cities.
- Evaluate recycling rates and recycling performance.
- Compare different waste disposal methods.
- Examine waste management costs.
- Identify relationships between waste generation, recycling rates, and other factors.
- Generate meaningful insights through exploratory data analysis.

## 📂 Dataset Information

**Dataset:** Waste Management and Recycling in India

The dataset was filtered to focus specifically on records where `waste_type` is Plastic.

Key features analyzed include:

- City / District
- Waste Generated (tons/day)
- Recycling Rate (%)
- Disposal Method
- Cost of Waste Management (₹/ton)
- Awareness Campaigns Count
- Landfill Capacity (tons)

## 🛠️ Technologies & Libraries Used

- **Python** – Data analysis and processing
- **Pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Jupyter Notebook** – Interactive analysis

## 🔍 Analysis Workflow

### 1. Data Loading and Exploration
- Imported the dataset using Pandas.
- Filtered the dataset to include only plastic waste records.
- Examined dataset structure, data types, statistical summaries, and unique values.

### 2. Data Cleaning
- Checked for missing values.
- Verified numerical features for outliers.
- No missing values or outliers were identified in the selected data, so no replacement or removal was required.

### 3. Feature Engineering
Created two additional features:

- **Recycled Waste:** Calculated the actual quantity of plastic waste recycled per day using waste generation and recycling rate.
- **Recycling Category:** Classified recycling performance into four categories:
  - Poor (0–40%)
  - Average (40–60%)
  - Good (60–80%)
  - Excellent (80–100%)

Removed selected columns that were not required for the subsequent analysis.

### 4. Exploratory Data Analysis (EDA)

**Univariate Analysis**
- Plastic waste generation distribution
- Disposal method distribution
- Waste management cost distribution
- Recycling rate distribution
- Landfill capacity distribution
- Recycling category distribution
- Recycled waste distribution

**Bivariate Analysis**
- City-wise average recycling rates
- Recycling rate by disposal method
- Top 10 cities by plastic waste generation
- Management cost by disposal method
- Recycling category by disposal method
- Awareness campaigns vs. recycling rate
- Management cost vs. recycling rate
- Waste generated vs. recycled waste

**Multivariate Analysis**
- Correlation heatmap of numerical features
- City-wise recycling rate by disposal method
- Management cost by recycling category and disposal method

## 📊 Key Findings

- Plastic waste generation varies significantly across cities, with some generating nearly 10,000 tons per day.
- The overall average recycling rate is approximately **58.14%**.
- **Indore** has the highest average recycling rate at **71.8%**, while **Vadodara** has the lowest at **41.8%**.
- **Lucknow** generates the highest average plastic waste at approximately **8,600 tons per day**.
- Recycling is the most economical disposal method at approximately **₹2,468 per ton**, despite having the lowest average recycling rate among the disposal methods analyzed.
- Awareness campaigns and waste management costs show only weak relationships with recycling performance.
- Waste generation and recycling rate are important factors in determining the quantity of plastic waste recycled.
- Recycling performance varies across cities and disposal methods, highlighting the need for city-specific waste management strategies.

## 📈 Data Visualizations

The project uses multiple visualizations to explore patterns and relationships in the dataset.

You can add exported charts from your Jupyter Notebook in the `images` folder.

Example:

```markdown
![Plastic Waste Distribution](images/waste_distribution.png)

![Recycling Rate Heatmap](images/recycling_heatmap.png)
```

## 📁 Project Structure

```text
Plastic-Waste-and-Recycling-Analytics/
│
├── images/
│   ├── waste_distribution.png
│   ├── recycling_heatmap.png
│   └── disposal_methods.png
│
├── Plastic Waste and Recycling Analysis.ipynb
├── Waste_Management_and_Recycling_India_cleaned.csv
└── README.md
```

## ▶️ How to Run the Project

1. Clone this repository:

```bash
git clone <your-repository-url>
```

2. Navigate to the project folder:

```bash
cd Plastic-Waste-and-Recycling-Analytics
```

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

4. Open Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `Plastic Waste and Recycling Analysis.ipynb` and run the cells.

**Note:** Keep the dataset in the project folder and update the notebook's CSV file path if necessary.

## 📝 Conclusion

This analysis provides insights into plastic waste generation, recycling efficiency, and waste management practices across Indian cities. The findings highlight variations in recycling performance and the importance of improving recycling strategies. The project demonstrates how exploratory data analysis and visualization can support data-driven understanding of environmental challenges.

---

**Project Category:** Data Analytics | Exploratory Data Analysis | Environmental Analytics

**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn
