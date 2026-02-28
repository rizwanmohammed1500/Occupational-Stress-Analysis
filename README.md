# Occupational Stress and Sleep Quality Analysis: An Independent Mini-Project By Rizwan Mohammed

## Project Overview
This project investigates the relationship between occupations and sleep quality. Using a dataset of 374 individuals, I performed data cleaning and exploratory data analysis (EDA) to identify how stress levels vary by job title and how high stress directly impacts sleep quality.

## Notes
* **Original Dataset:** The raw dataset I used for this project is **synthetic** and made for educational purposes. The patterns in the dataset **model real-world** clincal observations. It can be found here: [Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset/data)
* **Data Cleaning:** I found that the raw dataset had multiple errors, including incorrect entries (ex: The sleep disorder column used both "None" and "NaN" to represent no sleep disorder) and inconsistent values (the dataset used both "Normal" and "Normal Weight" under the BMI category).
* **Lack of Entries for Certain Occupations:** The dataset I used only featured 2 entries for Sales Representatives, 4 for Scientists and Software Engineers, and just 1 for Managers. This most likely skewed the findings, and more entries are needed for these occupations to provide an accurate analysis. As such, these findings should be treated as directional rather than definitive, even though they closely follow real-world patterns.

## Data Cleaning Process
1.  **Standardization:** Combined "Normal Weight" and "Normal" categories in BMI.
2.  **Improve Analysis:** Split the "Blood Pressure" column into two separate integer columns ("Systolic" and "Diastolic") for better correlational analysis.
3.  **Confirmation:** Performed `value_counts()` analysis to ensure no duplicate or misspelled categories remained.

## Visualizations and Graphs
* **Bar Graph:** I created a bar graph to show the average stress level across 11 different occupations. <img width="990" height="590" alt="bar graph" src="https://github.com/user-attachments/assets/e1de8bbb-6102-4d2d-98bb-575cfa1bc5f0" />
* **Boxplot:** I created a boxplot to show the distribution of sleep quality, highlighting the range and outliers for each level. <img width="678" height="471" alt="boxplot" src="https://github.com/user-attachments/assets/4807400d-7f5c-4fbb-94d5-6d7791d02bb7" />

## Tools Used (Google Colab)
* **Python**
* **Pandas:** Data manipulation and cleaning.
* **Seaborn/Matplotlib:** Statistical data visualization.

## Conclusion
* **Occupational Stress Rankings:** After analysis of the graphs and data, I found that in this particular group, Sales Representatives reported the highest average stress levels, while Software Engineers and Teachers reported the lowest (about 4). This indicates that certain roles, like Sales Representatives, have a "stress-premium' that inherently raises the stress levels of the person.
* **The Stress-Sleep Correlation:** I found a strong negative correlation between stress and sleep quality; as stress levels increase, sleep quality decreases. I discovered this after charting the cleaned data using the box plot in my project.
* **Future Steps:** Increasing the sample size of underrepresented occupations (Sales Representatives, Software Engineers, Scientists, and Managers) would provide more accurate analysis. In addition, Blood Pressure could be analyzed to discover the relationship between Systolic and Diastolic BP, sleep, and stress levels per occupation.
