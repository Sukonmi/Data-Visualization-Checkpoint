# 🎯OVERVIEW.
The Data Visualization Checkpoints is a series of steps designed to guide me through the process of exploring, analyzing, and visualizing a dataset. The checkpoint ensured that I cover the essential aspects of data visualization, from selecting appropriate chart types to answering specific analytical questions using visual tools. The primary goal was to transform raw data into meaningful insights that can be easily interpreted and communicated.

# 📢DESCRIPTION.
This Checkpoint involved the following:
In this checkpoint, I worked on the 'Climate change in Africa' dataset that was provided by the U.S global change research program.
- Dataset description : This dataset contains historical data about the daily min, max and average temperature fluctuation in 5 African countries (Egypt, Tunisia, Cameroon, Senegal, Angola) between 1980 and 2023.
- Initial Exploration.
- Selecting Appropriate Visuals.
- Creating Visualizations.
- Analysis and Interpretation.
- Summary and Insights.

# ℹ️INSTRUCTIONS.
- Load the dataset into a data frame using Python.
- Clean the data as needed.
- Plot a line chart to show the average temperature fluctuations in Tunisia and Cameroon. Interpret the results.
- Zoom in to only include data between 1980 and 2005, try to customize the axes labels.
- Create Histograms to show temperature distribution in Senegal between [1980,2000] and [2000,2023] (in the same figure). Describe the obtained results.
- Select the best chart to show the Average temperature per country.
- Make your own questions about the dataset and try to answer them using the appropriate visuals.

# 🛠️TOOLS USED.
- VSCode.
- Python.
- Jupyter Notebook.
- GitHub.
- Git.

```
import pandas as pd
import plotly.express as px

# Load the dataset
df = pd.read_csv('path_to_your_dataset.csv')

# Calculate the average temperature per country
avg_temp_per_country = climate_df.groupby("COUNTRY")["TAVG"].mean().reset_index()

# Plotting a Bar Chart with Plotly Express
fig = px.bar(avg_temp_per_country, x = "COUNTRY", y= "TAVG",
             title = "Average Temperature per Country (1980-2023)" ,
             labels = {"TAVG": "Average Temperature (°C)"},
             color = "COUNTRY")
fig.show()
```
 
