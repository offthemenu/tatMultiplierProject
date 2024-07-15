# slaCoefficientProject
Outline of How I Reconfigured One of My Previous Employer's Key Performance Indicators (KPIs)

TAT Multiplier: Enhancing KPI Effectiveness

<h2>Project Overview</h2>
This project is inspired by the narrative of a project manager's journey to improve Key Performance Indicators (KPIs) in a corporate setting. The main focus is on the development and implementation of the Turnaround Time (TAT) Multiplier to address discrepancies in the On-Time Delivery Percentage (OTD%) metric.

Table of Contents
Background
Installation
Usage
Project Structure
Data Processing Steps
Output Files
Contributing
License
Background
The project was inspired by the need to reassess the effectiveness of high-performing KPIs, particularly the On-Time Delivery Percentage (OTD%). The TAT Multiplier was developed to provide a more dynamic and insightful measure of vendor performance, addressing the limitations of static KPIs.

The full narrative detailing the inspiration and development process can be found on Medium.

Installation
To run this project, you'll need Python and the necessary packages. Install the required packages using:

bash
Copy code
pip install -r requirements.txt
Usage
To use the data processing script, run the Jupyter notebook dataProcessing.ipynb. This notebook includes all steps to process vendor data and calculate performance metrics.

Project Structure
dataProcessing.ipynb: Main Jupyter notebook with data processing and analysis code.
requirements.txt: List of required Python packages.
vendor_data.csv: Input data file with raw vendor performance data.
df_newTAT.csv: Output file with processed data and new TAT values.
vendor_scores.csv: Output file with vendor performance scores.
Data Processing Steps
Data Loading: Load raw vendor performance data from a CSV file.
Data Cleaning: Handle missing values, data type conversions, and outlier removal.
Feature Engineering: Calculate new features such as delivery score, error rate, and submission quality.
Data Analysis: Analyze processed data to evaluate vendor performance.
Scoring: Assign scores to vendors based on performance metrics.
Output Generation: Save processed data and vendor scores to CSV files.
Detailed Steps
Data Loading:

Load input CSV file using pandas.
Ensure correct data formatting.
Data Cleaning:

Handle missing values and data type conversions.
Remove outliers.
Feature Engineering:

Calculate delivery_score based on delivery time and other metrics.
Compute error_rate for submission quality.
Derive additional metrics for comprehensive vendor performance evaluation.
Data Analysis:

Perform exploratory data analysis (EDA).
Visualize insights using plots and graphs.
Scoring:

Develop a scoring algorithm for vendor performance.
Use calculated features to assign scores.
Output Generation:

Save processed DataFrame to df_newTAT.csv.
Save vendor performance scores to vendor_scores.csv.
Output Files
df_newTAT.csv: Processed vendor data with calculated TAT values.
vendor_scores.csv: Vendor performance scores.
Contributing
Contributions are welcome! Please follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature/YourFeature).
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature/YourFeature).
Open a Pull Request.
License
This project is licensed under the MIT License. See the LICENSE file for details.