# World Happiness Report: Data Handling & Visualization Project

This repository contains a college project focused on data handling and visualization using Python. The project analyzes the [World Happiness Report dataset from Kaggle](https://www.kaggle.com/datasets/yadiraespinoza/world-happiness-2015-2024) (2015-2024) to identify trends and correlations in global happiness.

The primary goal is to demonstrate the end-to-end process of taking raw, separate data files, cleaning them into a single usable dataset, and then creating insightful visualizations to answer key questions.

---

## 📈 Project Overview

### 1. Data Handling & Cleaning

The raw data was spread across 10 separate CSV files, each with different formatting issues. The handling portion of the script (`.py` file) performs the following tasks:

* **File Loading:** Loads 10 separate CSV files (one for each year, 2015-2024).
* **Delimiter Correction:** Correctly identifies the **semicolon (`;`)** as the file delimiter.
* **Decimal Correction:** Correctly identifies the **comma (`,`)** as the decimal separator (e.g., `7,597` -> `7.597`) and converts these columns to numeric (float) types.
* **Column Standardization:** Merges inconsistent column names from different years (e.g., `Happiness Score` and `Ladder score` are combined into a single `Score` column).
* **Data Aggregation:** Combines all 10 years of data into a single, clean Pandas DataFrame.
* **Missing Data:** Drops any rows with missing values to ensure visualization accuracy.

### 2. Data Visualization

The visualization portion of the script uses Matplotlib and Seaborn to answer three main questions.

---

## 📊 Visualizations

> **Note:** To make these images appear in your README, run the Python script, save the plots that pop up (right-click -> Save Image As...), upload them to your GitHub repository, and then update the file paths below.

### 1. How has average world happiness changed over time?

This line chart shows the average happiness score of all countries from 2015 to 2024.

![Average Happiness Over Time](path/to/your/line_chart.png)

### 2. Is there a relationship between a country's GDP and its happiness?

This scatter plot maps a country's Happiness Score against its GDP per capita for the year 2024. A regression line is included to show the correlation.

![Happiness vs GDP Scatter Plot](path/to/your/scatter_plot.png)

### 3. What were the top 10 happiest countries in 2024?

This horizontal bar chart ranks the 10 countries with the highest happiness scores in 2024.

![Top 10 Happiest Countries Bar Chart](path/to/your/bar_chart.png)

---

## 🛠️ Technologies Used

* **Python 3:** The core language for the project.
* **Pandas:** Used for all data loading, cleaning, and manipulation.
* **Matplotlib:** The fundamental library used for creating the plots.
* **Seaborn:** Used on top of Matplotlib for more aesthetic and complex statistical plots (like `regplot`).

---

## 🚀 How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git)
    ```

2.  **Install dependencies:**
    Make sure you have the required Python libraries installed.
    ```bash
    pip install pandas matplotlib seaborn
    ```

3.  **Get the data:**
    * Download the dataset from [Kaggle](https://www.kaggle.com/datasets/yadiraespinoza/world-happiness-2015-2024).
    * Unzip the files.
    * **Important:** Rename the files to match the script's pattern: `world_happiness_2015.csv`, `world_happiness_2016.csv`, etc.
    * Place all 10 CSV files in the same root folder as the Python script.

4.  **To Identify the exact/updated coloumn names run:**
    
    ```bash
    python1.py
    ```
    The script will print the updated name(if data update is made in future), later you can change the python2.py script accordingly.

5.  **Run the script:**
    
    ```bash
    python2.py
    ```
    The script will print status updates to the console and then display the three plots one by one.

---

---

## 📄 Data Source

* **Dataset:** World Happiness 2015-2024
* **Source:** [Kaggle](https://www.kaggle.com/datasets/yadiraespinoza/world-happiness-2015-2024)
* **Original Source:** World Happiness Report (via the Gallup World Poll)
