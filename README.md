# 📊 Google Play Store Apps & Reviews – Exploratory Data Analysis

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on Google Play Store application data and user reviews.

The objective is to analyze:

* App characteristics
* Ratings
* Reviews
* Installations
* Pricing
* Categories
* Content ratings
* User sentiment

The project uses two datasets:

1. **Google Play Store Apps Dataset**
2. **Google Play Store User Reviews Dataset**

The analysis is performed using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

---

## 🎯 Objectives

The main objectives of this project are:

* Analyze the distribution of Google Play Store applications.
* Identify the most common app categories.
* Analyze app ratings and review counts.
* Compare free and paid applications.
* Analyze app installations across categories.
* Study content rating distribution.
* Perform sentiment analysis on user reviews.
* Analyze sentiment polarity and subjectivity.
* Identify the most reviewed applications.
* Compare average ratings across categories.
* Analyze relationships between numerical variables using correlation analysis.

---

## 📂 Datasets

### 1. Google Play Store Apps Dataset

The Apps dataset contains information such as:

| Column             | Description                    |
| ------------------ | ------------------------------ |
| **App**            | Name of the application        |
| **Category**       | App category                   |
| **Rating**         | User rating                    |
| **Reviews**        | Number of reviews              |
| **Size**           | Application size               |
| **Installs**       | Number of installations        |
| **Type**           | Free or Paid                   |
| **Price**          | Application price              |
| **Content Rating** | Target audience/content rating |

### 2. Google Play Store User Reviews Dataset

The Reviews dataset contains:

| Column                     | Description                    |
| -------------------------- | ------------------------------ |
| **App**                    | Application name               |
| **Translated_Review**      | User review text               |
| **Sentiment**              | Positive, Negative, or Neutral |
| **Sentiment_Polarity**     | Sentiment polarity score       |
| **Sentiment_Subjectivity** | Sentiment subjectivity score   |

---

## 🛠️ Technologies Used

| Technology           | Purpose                        |
| -------------------- | ------------------------------ |
| **Python**           | Data analysis                  |
| **Pandas**           | Data manipulation and analysis |
| **NumPy**            | Numerical operations           |
| **Matplotlib**       | Data visualization             |
| **Seaborn**          | Statistical visualization      |
| **Jupyter Notebook** | Development and analysis       |
| **VS Code**          | Development environment        |

---

## 🔄 Project Workflow

```text
Data Collection
      ↓
Data Loading
      ↓
Data Inspection
      ↓
Data Cleaning
      ↓
Descriptive Statistics
      ↓
Exploratory Data Analysis
      ↓
Data Visualization
      ↓
Sentiment Analysis
      ↓
Apps + Reviews Integration
      ↓
Correlation Analysis
      ↓
Key Insights
```

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

* Removed invalid or shifted rows.
* Cleaned the `Installs` column.
* Converted installation values into numeric format.
* Converted app sizes into bytes.
* Converted reviews into numeric values.
* Removed `$` symbols from the `Price` column.
* Converted prices into numeric values.
* Removed missing translated reviews.
* Handled missing and invalid values.

These preprocessing steps prepare the datasets for accurate analysis and visualization.

---

## 📊 Exploratory Data Analysis

The project includes the following visualizations:

### 1. Top 15 App Categories

Analyzes the categories containing the highest number of applications.

### 2. Rating Distribution

Shows the distribution of application ratings.

### 3. Content Rating Distribution

Analyzes applications based on their content rating.

### 4. Top 10 Categories by Total Installs

Identifies categories with the highest total number of installations.

### 5. Free vs Paid App Rating Distribution

Compares ratings between free and paid applications using a boxplot.

### 6. Sentiment Distribution

Shows the distribution of:

* Positive reviews
* Negative reviews
* Neutral reviews

### 7. Sentiment Polarity vs Subjectivity

Analyzes the relationship between sentiment polarity and subjectivity.

### 8. Top 10 Most Reviewed Apps

Identifies applications with the highest number of user reviews.

### 9. Average Sentiment Polarity by Category

Analyzes average sentiment polarity across different app categories.

### 10. Average Rating by Category

Compares average application ratings across categories.

### 11. Correlation Heatmap

Examines relationships between:

* Rating
* Reviews
* Installs
* Sentiment Polarity
* Sentiment Subjectivity

---

## 💬 Sentiment Analysis

User reviews are analyzed based on their sentiment.

The project examines:

* **Positive Sentiment**
* **Negative Sentiment**
* **Neutral Sentiment**
* **Sentiment Polarity**
* **Sentiment Subjectivity**

Reviews with missing translated review text are removed before performing the analysis.

---

## 🔗 Data Integration

The Apps and Reviews datasets are merged using the **`App`** column.

```python
merged = pd.merge(
    reviews_clean,
    apps,
    on="App",
    how="inner"
)
```

The merged dataset allows app characteristics and user sentiment to be analyzed together.

---

## 📈 Key Analysis

The project calculates important metrics including:

* Total number of applications
* Total number of reviews
* Number of app categories
* Number of free applications
* Number of paid applications
* Average application rating
* Most common app category
* Category with the highest total installations
* Number of positive reviews
* Number of negative reviews
* Number of neutral reviews

---

## 🔑 Key Insights

The analysis helps answer questions such as:

* Which app categories contain the most applications?
* Which categories receive the highest number of installations?
* How are application ratings distributed?
* How do free and paid applications compare?
* Which applications receive the most reviews?
* What is the distribution of user sentiment?
* Which categories have higher average ratings?
* What relationships exist between ratings, reviews, and installations?
* What relationship exists between sentiment polarity and subjectivity?

---

## 📁 Project Structure

```text
Google-Play-Store-EDA/
│
├── data/
│   ├── googleplaystore.csv
│   └── googleplaystore_user_reviews.csv
│
├── notebooks/
│   └── EDA1.ipynb
│
├── visualizations/
│   └── charts/
│
├── README.md
│
└── requirements.txt
```

---

## ▶️ How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Navigate to the Project Folder

```bash
cd Google-Play-Store-EDA
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

Alternatively, open the project using **VS Code**.

### Step 5: Run the Analysis

Execute the notebook cells in sequence:

```text
Data Loading
      ↓
Data Cleaning
      ↓
Statistical Analysis
      ↓
Visualization
      ↓
Sentiment Analysis
      ↓
Data Integration
      ↓
Correlation Analysis
```

---

## 📌 Conclusion

This project provides an **end-to-end exploratory analysis** of Google Play Store applications and user reviews.

By combining application-level information with user sentiment data, the project provides insights into:

* Application categories
* Ratings
* Installations
* Pricing
* Reviews
* User sentiment

The project demonstrates practical skills in:

**Python • Data Cleaning • Exploratory Data Analysis • Data Visualization • Sentiment Analysis • Statistical Analysis**

---

## 👩‍💻 Author

### **Amisha**

**M.Tech – Computer Science Engineering**
**Aspiring Data Analyst**

### Skills Demonstrated

```text
Python
Pandas
NumPy
Matplotlib
Seaborn
Exploratory Data Analysis
Data Visualization
Sentiment Analysis
```

---

## ⭐ Acknowledgement

This project was developed as part of a **Data Analytics / Exploratory Data Analysis project** using Google Play Store application and user review datasets.
