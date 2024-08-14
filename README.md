# matplotlib_challenge5

# visualization-challenge-Pymaceuticals
This project furthers the analysis and visualization of real word data with Python in Pandas and Matplotlib. Summary statistics, correlation coefficients and linear regression modeling are also done.

The solutions is in the file pymaceuticals.ipynb, and data used is in the data folder in the root.

## Key findings were:

In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against Ramicane, Ketapril, Naftisol, Zoniferol, Placebo, Stelasyn, Ceftamin, Infubinol, and Propriva.

Mice treated with Capomulin and Ramicane had the highest numbers of mice points, exposure, compared to the rest of the drug regimen. Propriva had the least observed mouse points in the course of the study

Final tumor volumes were the least in Ramicane followed by Capomulin at at least 41.0 mm3 but highest in Ketapril at 55.88 mm3. Ketapril has also the highest variance in tumor volume as well as the highest standard deviation and SEM. Similar high distributions were seen in mice that were on Naftiso .-
Infubinol had potential outliers, and this may have skewed the overall mean volumes of mice exposed to this drug, suggesting that it might have had better efficacy than what what observed in the stu y- . Many mice that were on ceftamin were seen to have large final tumor volumes, and this may require further investigat o- n. In general, the size of the tumor appeared to reduce significantly between day 20 and 35 among mice on Capomulin. There was minimal remission between days 36 and 45. A strong positive correlation was thus observed between the study drug and the average tumour volume (84%), with lower doses proving better on SCC in the mice exposed to it.


## The Task

Prepare the data.

- Generate summary statistics.

- Create bar charts and pie charts.

- Calculate quartiles, find outliers, and create a box plot.

- Create a line plot and a scatter plot.

- Calculate correlation and regression.


## Prepare the Data
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

- Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

- Display the updated number of unique mice IDs.

## Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics:

- A row for each drug regimen. These regimen names should be contained in the index column.

- A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

## Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

- Create the first bar chart with the Pandas DataFrame.plot() method.

- Create the second bar chart with Matplotlib's pyplot methods.

- Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

- Create the first pie chart with the Pandas DataFrame.plot() method.

## Create the second pie chart with Matplotlib's pyplot methods.

- Calculate Quartiles, Find Outliers, and Create a Box Plot
- Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

- Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

- Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
