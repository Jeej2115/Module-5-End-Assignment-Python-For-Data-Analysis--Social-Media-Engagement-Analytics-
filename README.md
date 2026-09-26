# Module-5-End-Assignment-Python-For-Data-Analysis--Social-Media-Engagement-Analytics-
In this assignment, I will work with a social media dataset containing social media engagement metrics. The task involves data cleaning, transformation, NumPy/Pandas operations,exploratory data analysis, visualizations, and generating insights.

# Python Social Media Data Analysis & Visualization

## 📌 Project Overview

This project focuses on analyzing and visualizing **social media data using Python**. The objective is to explore user behavior, post performance, engagement patterns, sentiment, device usage, and other important factors that influence social media activity.

The project uses **Pandas, NumPy, Matplotlib, Seaborn, and Plotly** to clean, analyze, and visualize the dataset and generate meaningful insights.

---

## 🎯 Objectives

The main objectives of this project are:

* Clean and prepare social media data for analysis.
* Perform exploratory data analysis using Pandas.
* Analyze likes, comments, shares, impressions, and engagement.
* Study post performance across different content types and categories.
* Analyze user behavior based on age, verification status, and devices.
* Examine engagement and impressions based on posting time.
* Analyze sentiment and its relationship with engagement.
* Create static visualizations using Matplotlib and Seaborn.
* Create interactive visualizations using Plotly.
* Extract meaningful insights from the analyzed data.

---

## 🛠️ Technologies Used

| Technology       | Purpose                        |
| ---------------- | ------------------------------ |
| Python           | Programming and data analysis  |
| Pandas           | Data cleaning and manipulation |
| NumPy            | Numerical operations           |
| Matplotlib       | Data visualization             |
| Seaborn          | Statistical visualization      |
| Plotly           | Interactive visualization      |
| Jupyter Notebook | Development environment        |

---

## 📂 Dataset

The dataset contains social media post and user-related information.

### Important Columns

* `user_id` – Unique identifier of the user
* `age` – Age of the user
* `gender` – Gender of the user
* `country` – User's country
* `post_id` – Unique identifier of the post
* `post_type` – Type of social media post
* `post_category` – Category of the post
* `likes` – Number of likes received
* `comments` – Number of comments received
* `shares` – Number of shares received
* `watch_time_sec` – Watch time in seconds
* `impression_count` – Number of impressions
* `posted_at` – Date and time when the post was published
* `follower_count` – Number of followers
* `is_verified` – Verification status of the account
* `device_type` – Device used by the user
* `sentiment` – Sentiment associated with the post
* `hashtags` – Hashtags used in the post
* `engagement_rate` – Engagement rate of the post

---

## 🔄 Data Preparation

The dataset was inspected and prepared before performing analysis.

The major data preparation steps included:

1. Loading the dataset using Pandas.
2. Inspecting rows, columns, and data types.
3. Checking for missing values.
4. Checking for duplicate records.
5. Converting date/time columns into appropriate datetime format.
6. Creating additional columns required for analysis.
7. Grouping and aggregating data for analysis.

### Total Engagement

A new `engagement` column was created using:

```python
df["engagement"] = df["likes"] + df["comments"] + df["shares"]
```

This combines the major interaction metrics into a single engagement measure.

---

## 📊 Exploratory Data Analysis

The project explores several aspects of social media performance.

### Content Performance

The analysis examines:

* Average engagement by post type
* Average engagement by post category
* Average engagement rate by country
* Content categories with higher engagement
* Post types receiving greater interaction

### User Trends

The project analyzes:

* Relationship between age and engagement
* Engagement differences between verified and non-verified accounts
* Number of posts from verified and non-verified users
* User activity patterns

### Behavioral Insights

The analysis includes:

* Best time of day based on average impressions
* Average impressions by hour
* Morning, afternoon, evening, and night performance
* Watch time by device type
* Device usage patterns

### Sentiment Analysis

The project examines:

* Engagement by sentiment
* Engagement rate by sentiment
* Impressions by sentiment
* Performance of negative and neutral posts
* Likes, comments, and shares across sentiment categories

---

## 📈 Data Visualizations

### Matplotlib

The project includes visualizations such as:

* Scatter plot
* Line chart
* Relationship between engagement metrics
* Trends over time

### Seaborn

The project includes:

* Count plot for post types
* Bar plot for average likes by category
* Violin plot for followers and sentiment
* Pair plot for numerical features
* Heatmap for correlation analysis
* Swarm plot for engagement by device

### Plotly

Interactive visualizations were created to make the analysis easier to explore.

These include:

* Interactive line chart
* Interactive bar chart
* Interactive scatter chart
* Interactive bubble chart

---

## 🔍 Key Analysis Areas

### 1. Post Type Performance

Post types were grouped and compared based on their average engagement to identify differences in audience interaction.

### 2. Content Category Performance

Different content categories were analyzed using average engagement to understand how content themes perform.

### 3. Country-Level Engagement

Countries were compared using average engagement rates to identify differences in audience interaction across locations.

### 4. Age and Engagement

The relationship between user age and total engagement was analyzed using grouped statistics, correlation, and visualization.

### 5. Verified Account Performance

Verified and non-verified accounts were compared based on:

* Average engagement
* Engagement rate
* Number of posts

### 6. Posting Time Analysis

The `posted_at` column was used to extract the posting hour and analyze which periods received higher average impressions.

### 7. Device Analysis

Different device types were compared based on average watch time.

### 8. Sentiment Analysis

Posts were grouped by sentiment to examine how positive, negative, and neutral content performed across engagement metrics.

---

## 💡 Insights

The analysis helps identify patterns such as:

* Differences in engagement across post types.
* Differences in performance between content categories.
* Variations in engagement rates across countries.
* The relationship between age and social media engagement.
* Performance differences between verified and non-verified accounts.
* Posting periods associated with higher impressions.
* Differences in watch time across device types.
* How sentiment relates to engagement and impressions.

The exact findings depend on the values present in the dataset and the results generated during analysis.

---

## 📁 Project Structure

```text
Python-Social-Media-Data-Analysis/
│
├── Social_Media_Data_Analysis.ipynb
├── social_media_dataset.csv
├── README.md
└── visualizations/
```

---

## ▶️ How to Run the Project

### Step 1: Install Python

Install Python or Anaconda on your system.

### Step 2: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn plotly
```

### Step 3: Open Jupyter Notebook

```bash
jupyter notebook
```

or open the project using **JupyterLab**.

### Step 4: Load the Dataset

```python
import pandas as pd

df = pd.read_csv("social_media_dataset.csv")
```

### Step 5: Run the Notebook

Run the notebook cells sequentially to perform:

1. Data loading
2. Data inspection
3. Data cleaning
4. Feature creation
5. Exploratory analysis
6. Visualization
7. Interactive visualization
8. Insight generation

---

## 🧰 Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
```

---

## 📌 Learning Outcomes

Through this project, I developed practical knowledge of:

* Python data analysis
* Pandas DataFrame operations
* Data cleaning and preprocessing
* GroupBy and aggregation
* Feature creation
* Date/time analysis
* Correlation analysis
* Matplotlib visualization
* Seaborn statistical visualization
* Plotly interactive visualization
* Exploratory Data Analysis (EDA)
* Extracting insights from real-world datasets

---

## 📝 Conclusion

This **Python Social Media Data Analysis & Visualization project** provided practical experience in analyzing social media data using Python. The project covered the complete workflow from data loading and preparation to exploratory analysis and visualization.

Using **Pandas and NumPy**, the data was cleaned, transformed, and analyzed. **Matplotlib and Seaborn** were used to create meaningful statistical and exploratory visualizations, while **Plotly** was used to create interactive charts.

The analysis explored content performance, user trends, posting behavior, device usage, engagement, impressions, and sentiment. These analyses demonstrate how Python can be used to transform raw social media data into meaningful information that can support data-driven understanding and decision-making.

Overall, this project strengthened my skills in **Python, data analysis, visualization, exploratory data analysis, and interpreting data-driven insights**.

