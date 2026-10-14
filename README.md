Healthcare Data Exploratory Data Analysis (EDA)
📌 Project Overview
This project explores healthcare data using Python to understand patient admissions, medical conditions, billing amounts, hospital stay duration, and admission trends over time. The notebook uses data cleaning, descriptive statistics, grouping, cross-tabulation, and visualizations to identify patterns in the dataset.
🎯 Objectives
- Inspect the dataset structure, columns, and missing values.
- Clean and standardize admission-type values.
- Convert admission and discharge dates into datetime format.
- Calculate the length of each hospital stay.
- Summarize billing amounts and average patient age by medical condition.
- Compare medical conditions with gender and admission type.
- Visualize billing distributions and monthly patient admissions.
- Explore correlations among age, stay duration, and billing amount.
🛠️ Tools and Libraries
- Python — analysis and scripting
- Pandas — data loading, cleaning, grouping, and time-series resampling
- NumPy — numerical computing
- Matplotlib — charts and plots
- Seaborn — statistical visualizations
- Jupyter Notebook / Google Colab — interactive analysis environment
📂 Project Structure
.
├── eda5 og.ipynb       # Jupyter notebook containing the analysis
├── healthcare_data.csv # Input dataset (add this file if you are permitted to share it)
└── README.md           # Project documentation
The notebook loads the dataset from /content/healthcare_data.csv, which is a Google Colab-style path. Upload healthcare_data.csv to your Colab session or update the file path when running locally. Only publish the dataset if you have permission to share it and it contains no sensitive patient information.

🔍 Analysis Workflow
1. Load the data — import the required libraries and read the CSV file with Pandas.
2. Inspect the dataset — view sample rows, dataset dimensions, data types, and missing-value counts.
3. Clean admission types — remove extra whitespace and standardize capitalization in Admission_Type.
4. Prepare dates — convert Date_of_Admission and Discharge_Date to datetime values and examine date components.
5. Create a stay-duration feature — calculate stay_days from discharge date minus admission date.
6. Perform descriptive analysis — summarize Billing_Amount and calculate mean age by Medical_Condition.
7. Compare categories — use cross-tabulations and grouped counts to examine medical condition, gender, and admission type.
8. Visualize patterns — create bar charts, stacked billing charts, violin plots, monthly admission trends, and a correlation heatmap.
📊 Visualizations Included
- Admission Type Counts: number of records in each admission category.
- Admission Type by Medical Condition: stacked bar chart comparing admission categories across conditions.
- Total Billing by Medical Condition and Admission Type: stacked bar chart of summed billing amounts.
- Billing Amount Distribution: violin plot showing billing distributions by medical condition.
- Monthly Patient Admissions: time-series line chart of monthly admission counts.
- Correlation Heatmap: correlations among Age, stay_days, and Billing_Amount.
▶️ How to Run
Option 1: Google Colab
1. Upload eda5 og.ipynb to Google Colab.
2. Upload the required healthcare_data.csv file to the Colab session.
3. Confirm that the CSV path matches /content/healthcare_data.csv.
4. Run the notebook cells from top to bottom.
Option 2: Run Locally
1. Install Python and Jupyter Notebook, or use VS Code with the Jupyter extension.
2. Place the notebook and dataset in your project folder.
3. Install the dependencies:
   pip install pandas numpy matplotlib seaborn jupyter
4. Change the CSV path in the notebook to the local file path, for example:
   df = pd.read_csv("healthcare_data.csv")
5. Open the notebook and run all cells in order.
📁 Dataset Fields Used
The notebook references these columns:
- Age
- Medical_Code
- Medical_Condition
- Gender
- Admission_Type
- Date_of_Admission
- Discharge_Date
- Billing_Amount
It also creates a derived column, stay_days, representing the difference in days between discharge and admission dates.
💡 Key Skills Demonstrated
- Exploratory Data Analysis (EDA)
- Data cleaning and type conversion
- Feature creation with date calculations
- Descriptive statistics and aggregation
- Categorical comparisons using cross-tabulation
- Time-series resampling
- Data visualization and correlation analysis
⚠️ Notes and Limitations
- This notebook performs exploratory analysis; it does not train a machine-learning prediction model.
- The README does not report numerical findings because the dataset output values are not documented here. Run the notebook to obtain results for your copy of the data.
- Correlation indicates association, not causation.
- Ensure the dataset is anonymized and safe to publish before uploading it to a public repository.
