<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

<h1>TAT Multiplier: Enhancing KPI Effectiveness</h1>

<h2>Project Overview</h2>
<p>This project is inspired by the narrative of a project manager's journey to improve Key Performance Indicators (KPIs) in a corporate setting. The main focus is on the development and implementation of the Turnaround Time (TAT) Multiplier to address discrepancies in the On-Time Delivery Percentage (OTD%) metric.</p>

<h2>Table of Contents</h2>
<ul>
  <li><a href="#background">Background</a></li>
  <li><a href="#installation">Installation</a></li>
  <li><a href="#usage">Usage</a></li>
  <li><a href="#project-structure">Project Structure</a></li>
  <li><a href="#data-processing-steps">Data Processing Steps</a></li>
  <li><a href="#output-files">Output Files</a></li>
  <li><a href="#contributing">Contributing</a></li>
  <li><a href="#license">License</a></li>
</ul>

<h2 id="background">Background</h2>
<p>The project was inspired by the need to reassess the effectiveness of high-performing KPIs, particularly the On-Time Delivery Percentage (OTD%). The TAT Multiplier was developed to provide a more dynamic and insightful measure of vendor performance, addressing the limitations of static KPIs.</p>
<p>The full narrative detailing the inspiration and development process can be found on <a href="https://medium.com/@personal.ianchang/why-your-kpis-might-need-a-facelift-especially-the-high-performing-ones-part-1-prologue-28f0dbdea24d">Medium</a>.</p>

<h2 id="usage">Usage</h2>
<p>To use the data processing script, run the Jupyter notebook <code>dataProcessing.ipynb</code>. This notebook includes all steps to process vendor data and calculate performance metrics.</p>

<h2 id="project-structure">Project Structure</h2>
<ul>
  <li><code>dataProcessing.ipynb</code>: Main Jupyter notebook with data processing and analysis code.</li>
  <li><code>requirements.txt</code>: List of required Python packages.</li>
  <li><code>vendor_data.csv</code>: Input data file with raw vendor performance data.</li>
  <li><code>df_newTAT.csv</code>: Output file with processed data and new TAT values.</li>
  <li><code>vendor_scores.csv</code>: Output file with vendor performance scores.</li>
</ul>

<h2 id="data-processing-steps">Data Processing Steps</h2>
<ol>
  <li><strong>Data Loading</strong>: Load raw vendor performance data from a CSV file.</li>
  <li><strong>Data Cleaning</strong>: Handle missing values, data type conversions, and outlier removal.</li>
  <li><strong>Feature Engineering</strong>: Calculate new features such as delivery score, error rate, and submission quality.</li>
  <li><strong>Data Analysis</strong>: Analyze processed data to evaluate vendor performance.</li>
  <li><strong>Scoring</strong>: Assign scores to vendors based on performance metrics.</li>
  <li><strong>Output Generation</strong>: Save processed data and vendor scores to CSV files.</li>
</ol>

<h3>Detailed Steps</h3>
<ol>
  <li><strong>Data Loading</strong>: 
    <ul>
      <li>Load input CSV file using <code>pandas</code>.</li>
      <li>Ensure correct data formatting.</li>
    </ul>
  </li>
  <li><strong>Data Cleaning</strong>: 
    <ul>
      <li>Handle missing values and data type conversions.</li>
      <li>Remove outliers.</li>
    </ul>
  </li>
  <li><strong>Feature Engineering</strong>: 
    <ul>
      <li>Calculate <code>delivery_score</code> based on delivery time and other metrics.</li>
      <li>Compute <code>error_rate</code> for submission quality.</li>
      <li>Derive additional metrics for comprehensive vendor performance evaluation.</li>
    </ul>
  </li>
  <li><strong>Data Analysis</strong>: 
    <ul>
      <li>Perform exploratory data analysis (EDA).</li>
      <li>Visualize insights using plots and graphs.</li>
    </ul>
  </li>
  <li><strong>Scoring</strong>: 
    <ul>
      <li>Develop a scoring algorithm for vendor performance.</li>
      <li>Use calculated features to assign scores.</li>
    </ul>
  </li>
  <li><strong>Output Generation</strong>: 
    <ul>
      <li>Save processed DataFrame to <code>df_newTAT.csv</code>.</li>
      <li>Save vendor performance scores to <code>vendor_scores.csv</code>.</li>
    </ul>
  </li>
</ol>

<h2 id="output-files">Output Files</h2>
<ul>
  <li><code>df_newTAT.csv</code>: Processed vendor data with calculated TAT values.</li>
  <li><code>vendor_scores.csv</code>: Vendor performance scores.</li>
</ul>

<h2 id="contributing">Contributing</h2>
<p>Contributions are welcome! Please follow these steps:</p>
<ol>
  <li>Fork the repository.</li>
  <li>Create a new branch (<code>git checkout -b feature/YourFeature</code>).</li>
  <li>Commit your changes (<code>git commit -m 'Add some feature'</code>).</li>
  <li>Push to the branch (<code>git push origin feature/YourFeature</code>).</li>
  <li>Open a Pull Request.</li>
</ol>

<h2 id="license">License</h2>
<p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for details.</p>

</body>
</html>
