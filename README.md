# Netflix Data Analysis & Visualization

This project offers a comprehensive exploration of the Netflix titles dataset, showcasing a wide range of data manipulation and visualization techniques using Python's powerful data science libraries. It serves as a practical demonstration of how to take a raw dataset, clean it, analyze it, and extract meaningful insights.

The analysis is available in two separate Jupyter Notebooks, with tasks and comments provided in both **English** and **Persian**.


## 🚀 About The Project

The goal of this project is to analyze the `netflix_titles.csv` dataset to understand the distribution of content, identify trends, and answer specific questions about the Netflix library. The entire analysis is conducted within a Jupyter Notebook, leveraging the capabilities of **pandas** for data manipulation, and **matplotlib** and **seaborn** for creating insightful visualizations.

The notebook is structured in a clear, **question-and-answer format**, where each section poses a data-related question and then provides the code to solve it. This makes it an excellent resource for anyone looking to practice or understand the fundamentals of data analysis in Python.

## 🛠️ Key Learnings & Skills Demonstrated

This project covers a wide array of essential data analysis skills, from initial data cleaning to advanced visualization.

### **Data Cleaning & Preprocessing**

-   **Data Loading:** Reading a CSV file into a pandas DataFrame and setting an index column.
-   **Initial Inspection:** Using `.info()`, `.isna().sum()`, and `.dtypes` to understand the dataset's structure, data types, and identify missing values.
-   **Handling Duplicates:** Finding and removing duplicate entries to ensure data integrity.
-   **Managing Missing Data:** Dropping rows with null values in critical columns (`.dropna()`) and imputing missing numerical data with the mean of a group.
-   **Data Type Conversion:** Converting columns to appropriate data types, such as transforming the `date_added` string column to a datetime object.
-   **String Manipulation & Extraction:** Using pandas string methods like `.str.extract()`, `.str.split()`, and `.str.contains()` to clean and extract valuable information from text-based columns like `duration` and `cast`.

---

### **Data Analysis & Manipulation**

-   **Grouping & Aggregation:** Utilizing `.groupby()` to segment the data and perform calculations on specific groups (e.g., calculating the average movie duration per rating).
-   **Filtering & Querying:** Slicing and filtering the DataFrame to isolate data that meets specific criteria, such as finding all titles starring "Brad Pitt".
-   **Data Reshaping:** Transforming the data's structure using `.melt()` to facilitate analysis and visualization, particularly for handling the 'country' column with multiple entries.
-   **Feature Engineering:** Creating new columns from existing data, such as extracting the year, month, day, and day of the week from the `date_added` column.
-   **One-Hot Encoding:** Converting the categorical `type` column into a numerical format using `pd.get_dummies()`, preparing the data for machine learning models.

---

### **Data Visualization**

This project emphasizes the power of visualization in storytelling with data:

-   **Bar Charts:** To compare the number of productions across the top 30 countries.
-   **Histograms & KDE Plots:** To analyze the distribution of movie durations and assess its normality.
-   **Pie Charts:** To visualize the proportion of content added on different days of the week for Movies, TV Shows, and both.
-   **Heatmaps:** A heatmap is used to show the frequency of content types for each rating, providing a clear visual comparison.
-   **Countplots:** To compare the distribution of ratings between Movies and TV Shows.
-   **Word Clouds:** Generating a visually engaging word cloud from movie/TV show titles and descriptions to highlight the most frequent and prominent words.

## 🏁 Getting Started

To run this project on your local machine or on Google Colab, follow these simple steps.

### **Suggested File Names**

To better reflect the content and bilingual nature of the project, here are some suggested file names for your notebooks:

-   **English Notebook:** `Netflix_Data_Analysis_EN.ipynb`
-   **Persian Notebook:** `Netflix_Data_Analysis_FA.ipynb`

### **Running Locally**

1.  **Prerequisites:**
    * Python 3.x
    * Jupyter Notebook or JupyterLab

2.  **Installation:**
    * Clone the repository:
        ```sh
        git clone [https://github.com/hmdrzam/netflix-data-analysis](https://github.com/hmdrzam/netflix-data-analysis)
        ```
    * Navigate to the project directory:
        ```sh
        cd project-directory
        ```
    * Install the required libraries:
        ```sh
        pip install pandas matplotlib seaborn wordcloud jupyterlab
        ```
    * Launch JupyterLab and open the notebook file of your choice.
        ```sh
        jupyter lab
        ```

### **Running on Google Colab**

You can also run this project directly in your browser using Google Colab, which requires no local setup.

1.  Open [Google Colab](https://colab.research.google.com/).
2.  Click on **File -> Upload notebook**.
3.  Upload either the English or Persian `.ipynb` file.
4.  You will also need to upload the `netflix_titles.csv` file to your Colab environment for the notebook to access it. You can do this by clicking on the folder icon in the left-hand sidebar and selecting "Upload to session storage".