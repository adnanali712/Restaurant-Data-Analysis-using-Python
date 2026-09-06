# 🍽️ Restaurant Data Analysis using Python

## 📊 Project Preview

Here are some of the visualizations generated during the analysis:

### 🔹 Cuisine Analysis
<img width="581" height="527" alt="analysis_1" src="https://github.com/user-attachments/assets/e3b42994-5930-4e2c-bd31-33323f73ae64" />


### 🔹 City / Restaurant Analysis

<img width="575" height="454" alt="analysis_4" src="https://github.com/user-attachments/assets/8d6a5147-37d9-474a-91b4-028285dab668" />



### 🔹 Price Range Analysis

<img width="581" height="454" alt="analysis_2" src="https://github.com/user-attachments/assets/969723da-9dfc-47ef-8118-c89b6c2b656d" />



### 🔹 Online Delivery Analysis

<img width="567" height="454" alt="analysis_3" src="https://github.com/user-attachments/assets/5c489a8a-a6b7-4602-9472-9185f2bdb45f" />




---

## 📁 Dataset

## 📊 Dataset Preview

The project uses a restaurant dataset containing **9,551 records and 21 columns**.

Here is a small preview of the dataset:

| Restaurant Name     | City      | Cuisines              | Average Cost for Two | Price Range | Aggregate Rating | Votes |
| ------------------- | --------- | --------------------- | -------------------: | ----------: | ---------------: | ----: |
| The Salt Restaurant | Abu Dhabi | Italian, European     |                   80 |           3 |              4.0 |   500 |
| Cafe Coffee Day     | Bangalore | Cafe, Desserts        |                  500 |           2 |              3.6 |   250 |
| Mainland China      | Bangalore | Chinese, Asian        |                 1500 |           4 |              4.2 |  1200 |
| Barbeque Nation     | Hyderabad | North Indian, BBQ     |                 1600 |           4 |              4.5 |  2500 |
| Paradise            | Hyderabad | Biryani, North Indian |                  800 |           3 |              4.1 |  1800 |

> **Note:** This table is only a small preview. The complete dataset is available in `Dataset (1).csv`.






## 🛠️ Technologies Used

* 🐍 Python
* 🐼 Pandas
* 📊 Matplotlib
* 📓 Jupyter Notebook
* 📁 CSV Dataset

---

# 🔎 Analysis Performed

## Level 1

### 1️⃣ Top Cuisines

The first analysis identifies the **most common cuisines** available in the dataset.

### Steps:

* Extracted the `Cuisines` column.
* Split restaurants containing multiple cuisines.
* Used `explode()` to separate individual cuisines.
* Counted cuisine occurrences using `value_counts()`.
* Identified the top 3 cuisines.
* Visualized the results using a bar chart.

**Pandas concepts used:**

* `dropna()`
* `str.split()`
* `explode()`
* `value_counts()`

---

### 2️⃣ City Analysis

The city analysis explores the number of restaurants and their average ratings across different cities.

### Analysis performed:

* Counted restaurants by city.
* Identified cities with the highest number of restaurants.
* Calculated the average restaurant rating for each city.
* Sorted cities based on their average rating.
* Identified the highest-rated city.

**Pandas concepts used:**

* `value_counts()`
* `groupby()`
* `mean()`
* `sort_values()`
* `idxmax()`

---

### 3️⃣ Price Range Distribution

This analysis examines how restaurants are distributed across different price ranges.

### Analysis performed:

* Counted restaurants for each price range.
* Calculated the percentage distribution.
* Created a bar chart showing the number of restaurants in each price category.

**Concepts used:**

* `value_counts()`
* Percentage calculation
* Matplotlib bar charts

---

### 4️⃣ Online Delivery Analysis

This section investigates the relationship between online delivery availability and restaurant ratings.

### Analysis performed:

* Counted restaurants with and without online delivery.
* Calculated the percentage of restaurants offering online delivery.
* Calculated the average rating based on online delivery availability.
* Visualized average ratings using a bar chart.

**Concepts used:**

* `value_counts()`
* `groupby()`
* `mean()`
* Matplotlib

---

# 📈 Level 2

## 1️⃣ Cuisine Combination Analysis

This analysis explores restaurants offering combinations of multiple cuisines.

### Analysis performed:

* Counted frequently occurring cuisine combinations.
* Calculated average ratings for cuisine combinations.
* Counted the number of restaurants for each combination.
* Filtered combinations having at least 10 restaurants.
* Identified highly rated cuisine combinations.

**Concepts used:**

* `value_counts()`
* `groupby()`
* `agg()`
* `mean()`
* Filtering

---

## 2️⃣ Geographic Analysis

The geographic analysis visualizes where restaurants are located using their latitude and longitude.

### Analysis performed:

* Used `Latitude` and `Longitude` columns.
* Created a scatter plot.
* Visualized the geographic distribution of restaurants.

**Visualization:**

A scatter plot was used to understand the geographical spread of restaurants.

---

## 3️⃣ Restaurant Chain Analysis

This analysis identifies restaurants that appear multiple times in the dataset and can therefore represent restaurant chains or repeated restaurant entries.

### Analysis performed:

* Counted occurrences of each restaurant name.
* Identified restaurant names appearing more than once.
* Calculated average ratings for restaurant names.

**Concepts used:**

* `value_counts()`
* `groupby()`
* `mean()`

---

## 4️⃣ Restaurant Rating Analysis

The dataset does not contain actual written customer review text.

Instead, it contains a categorical `Rating text` field.

Examples of rating categories include:

* Excellent
* Very Good
* Good
* Average
* Poor

The project analyzes the distribution of these rating categories and visualizes them using a bar chart.

### Data Validation

Because the dataset does not contain free-text reviews, the following analyses cannot be performed using this dataset:

* Review keyword frequency
* Average review length
* Review length versus rating

An additional dataset containing actual customer review text would be required for these analyses.

---

# 📊 Key Data Analysis Techniques

This project demonstrates practical use of:

```text
Pandas
│
├── Data Loading
├── Data Selection
├── Missing Value Handling
├── String Processing
├── value_counts()
├── groupby()
├── agg()
├── mean()
├── sort_values()
├── idxmax()
└── Data Filtering

Matplotlib
│
├── Bar Charts
└── Scatter Plots
```

---

# 📂 Project Structure

```text
Restaurant-Data-Analysis/
│
├── DATA ANALYST PYTHON PROJECT.ipynb
├── Dataset (1).csv
└── README.md
```

---

# 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### 2. Install required libraries

```bash
pip install pandas matplotlib jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open

```text
DATA ANALYST PYTHON PROJECT.ipynb
```

### 5. Update the dataset path

Make sure the notebook points to the CSV file included in the repository.

For example:

```python
import pandas as pd

df = pd.read_csv("Dataset (1).csv")
```

---

# 🎯 Project Objectives

The main objectives of this project are:

* Analyze restaurant data using Python.
* Identify the most popular cuisines.
* Analyze restaurant distribution across cities.
* Understand restaurant price ranges.
* Analyze online delivery availability.
* Explore cuisine combinations.
* Visualize geographic restaurant distribution.
* Identify repeated restaurant names and potential chains.
* Analyze restaurant rating categories.
* Practice Pandas and Matplotlib for real-world data analysis.

---

# 💡 Skills Demonstrated

Through this project, I practiced:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Data Manipulation
* Data Aggregation
* Data Visualization
* Statistical Analysis
* String Manipulation
* Data Validation
* Python Programming
* Pandas
* Matplotlib

---

# 📌 Conclusion

This project provided hands-on experience in analyzing a real-world restaurant dataset using Python.

The analysis explored **cuisines, cities, pricing, online delivery, geographic distribution, restaurant chains, and ratings**, while also demonstrating how to identify limitations in a dataset when required information, such as actual customer review text, is unavailable.

Overall, this project strengthened my practical understanding of **Python-based Data Analysis and Exploratory Data Analysis (EDA)**.

---

## 👨‍💻 Author

**Adnan**

Aspiring Data Analyst | Python | SQL | Excel | Power BI

---

⭐ If you find this project useful, feel free to star the repository!
