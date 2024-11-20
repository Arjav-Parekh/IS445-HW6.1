---
layout: default
title: Arjav Parekh - parekh6
---

# IS445 Data Visualization - HW6.1 

This page contains visualizations of the licenses dataset, along with a detailed analysis write-up.

## Visualizations

### Bar Chart: Count of Licenses by Ever Disciplined
The bar chart visualizes the distribution of licenses based on whether individuals have ever been disciplined. The data is grouped by the Ever Disciplined column, which contains two categories: "Yes" and "No". The y-axis represents the number of licenses in each category, while the x-axis categorizes the individuals based on their disciplinary status.

**Data Transformations**: To create the bar chart, I first performed a data transformation on the cleaned dataset by grouping the data based on the Ever Disciplined column. This column contains categorical values indicating whether an individual has ever been disciplined ("Yes" or "No"). Using the groupby function, I aggregated the data by counting the number of licenses in each category. This transformation resulted in a new DataFrame that consists of two columns: Ever Disciplined and the calculated License Count, representing the number of licenses in each disciplinary category. By resetting the index, I ensured the grouped data was in a format suitable for visualization with Altair.

**Design Choices**: The bar chart uses the Ever Disciplined column on the x-axis (nominal) and License Count on the y-axis (quantitative) to compare the number of licenses between disciplined ("Yes") and non-disciplined ("No") categories. A blue color scheme was applied to distinguish the bars, enhancing visual appeal and clarity. Tooltips were added to display exact values on hover, improving interactivity without cluttering the visualization. The chart title clearly communicates its purpose, while the size was chosen for optimal readability, making the chart both functional and visually engaging.

[View the Bar Chart](./assets/bar_chart.html)

---

### Interactive Bar Chart: Number of Licenses by License Type


**Data Transformations**: To create the interactive bar plot, the dataset was grouped by License Type to calculate the count of licenses for each type. Using the groupby function, the data was aggregated, and a new column, License Count, was created to represent the number of licenses for each License Type. The transformed dataset was then reset to ensure compatibility with Altair for visualization. This process simplified the data structure while preserving the necessary details for analysis.

**Design Choices**: The interactive bar chart visualizes License Type on the y-axis (nominal) and License Count on the x-axis (quantitative), providing a clear comparison of license types by their respective counts. The bars are colored using a blue gradient to reflect the number of licenses, emphasizing higher counts. Interactivity was added through tooltips, allowing users to hover over each bar to view exact values, enhancing the chart's usability. The axes are labeled descriptively, and the chart title succinctly conveys its focus, while its dimensions ensure readability across different screens. These choices make the visualization both informative and engaging for users.

[View the Interactive Bar Chart](./assets/interactive_bar_chart.html)

---

## Links to Resources

- [The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv)
- [The Analysis](./viz.ipynb)
