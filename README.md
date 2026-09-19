# 🍔 Zomato Data Analysis

A data analysis project analyzing Zomato restaurant performance to uncover key factors driving customer ratings, online ordering adoption, vote distributions, and average dining costs.

---

## 📊 Overview & Key Insights

By analyzing restaurant listings, ratings, and customer votes, this project highlights key patterns in restaurant success:

- **Online Ordering Impact:** Boxplot distributions show that restaurants offering online delivery consistently maintain higher average customer ratings.
- **Top Voted Restaurant:** *Empire Restaurant* received the highest total vote volume across the dataset.
- **Category Preferences:** Line plots and count plots reveal vote distribution across various restaurant types (Buffet, Cafes, Dining, etc.).
- **Pricing & Category Mapping:** Heatmaps illustrate the relationship between restaurant types, average cost for two, and online order availability.

---

## 🛠️ Tools & Libraries Used

- **Python**
- **Pandas** – Data loading, missing value checks, and string manipulation/type conversion
- **Matplotlib & Seaborn** – Visualizations (Histograms, Count plots, Boxplots, and Heatmaps)

---

## 📁 Dataset & Features

The dataset (`Zomato-data-.csv`) contains the following key fields:

| Field | Description |
| :--- | :--- |
| `name` | Name of the restaurant |
| `online_order` | Whether online ordering is available (`Yes`/`No`) |
| `book_table` | Table reservation option (`Yes`/`No`) |
| `rate` | Customer rating (cleaned from string format like `4.1/5` to float `4.1`) |
| `votes` | Total customer votes received |
| `approx_cost(for two people)` | Estimated cost for two diners |
| `listed_in(type)` | Restaurant category (e.g., Buffet, Cafe, Dining) |

---

## ⚙️ Data Preprocessing & Workflow

1. **Data Cleaning:** Custom function (`handle_rate`) to remove denominator characters (`/5`) and cast rating values to `float64`.
2. **Missing Values Check:** Verified zero missing values across all columns using `.isnull().sum()`.
3. **Exploratory Visualizations:**
   - **Distribution of Ratings:** Histogram analysis of overall ratings.
   - **Order Mode vs. Rating:** Boxplot comparing rated performance for online vs. offline ordering.
   - **Order Type Heatmap:** Pivot table and heatmap analyzing online ordering prevalence across restaurant types.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/r4rupesh/zomato-data-analysis-python.git
   cd zomato-data-analysis-pyton
