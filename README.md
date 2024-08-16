# Analyzing California High School SAT Performance vs. Poverty Level

## Overview
This project explores the relationship between SAT performance and the poverty level of students in California high schools. Poverty level is approximated by the percentage of students eligible for free and reduced-price lunch (FRPM). Using the provided datasets, the project analyzes correlations between SAT scores and poverty indicators and visualizes these relationships with various plots.

## Datasets
The analysis uses two main datasets:

- **SAT Scores Data (2014)**: Contains SAT performance details, including the number of test takers and average scores in reading, writing, and math.
- **FRPM Data (2014)**: Contains the percentage of students eligible for free and reduced-price lunch, a common proxy for poverty.

## Code Summary
The script performs the following steps:

1. **Loading Data**:
    - SAT and FRPM data are loaded into separate pandas DataFrames.

2. **Filtering SAT Data**:
    - Schools with fewer than 20 SAT test takers are excluded from the analysis to ensure the reliability of the results.

3. **Warmup Analysis**:
    - Correlation between SAT reading and writing scores is visualized using a scatter plot.
    - Correlation between SAT writing and math scores is similarly visualized.

4. **Merging Datasets**:
    - The SAT and FRPM datasets are merged on the `cds` column, which uniquely identifies each school.

5. **Analyzing Relationship Between Poverty and SAT Scores**:
    - A scatter plot is created to analyze the relationship between the percentage of students eligible for FRPM and the percentage of students scoring above 1500 on the SAT.
    - A trendline is added to visualize the overall trend in the data.

6. **Distribution Analysis**:
    - Histograms are plotted to visualize the distribution of SAT scores and FRPM eligibility across schools.
    - A comparison of SAT scores is made between schools with less than 10% FRPM eligibility and those with 10% or more.

## Visualizations
The following visualizations are generated:

- **Scatter Plots**:
    - Reading vs. Writing SAT Scores: Highlights the strong correlation between these two scores.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image1.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>
    - Writing vs. Math SAT Scores: Displays the correlation between writing and math scores.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image2.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>

- **Scatter Plot with Trendline**:
    - Poverty vs. SAT Scores: Shows the relationship between poverty levels (FRPM eligibility) and the percentage of students scoring 1500 or higher on the SAT.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image3.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>

- **Histograms**:
    - SAT Scores Distribution: Visualizes the distribution of SAT scores across schools.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image4.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>
    - FRPM Eligibility Distribution: Visualizes the distribution of FRPM eligibility across schools.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image5.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>
    - SAT Scores Comparison: Compares SAT score distributions between schools with low (<10%) and high (10%+) FRPM eligibility.
<p align="center">
  <img src="https://github.com/Sherryyy00/CA-SAT-Poverty-Analysis/blob/main/Graphs/image6.png", alt=" Daily Bar Chart " width="50%"         height="50%">
</p>

## How to Run
1. **Clone the Repository**:
    ```bash
    git clone <repository_url>
    cd <repository_folder>
    ```

2. **Install Required Libraries**:
    ```bash
    pip install pandas matplotlib numpy
    ```

3. **Run the Analysis**:
    - Open the script or notebook containing the analysis in your preferred Python IDE (e.g., Jupyter Notebook) and execute the code.

## Conclusion
The analysis suggests a negative relationship between poverty levels and SAT performance in California high schools. Schools with higher percentages of students eligible for FRPM tend to have lower percentages of students scoring above 1500 on the SAT.
