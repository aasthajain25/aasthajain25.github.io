---
name: IS 445 Homework 8
tools: [Python, HTML, vega-lite]
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# IS 445 Homework 8

### Dataset : Buildings dataset

### Plot 1 
{% include elements/button.html link="https://github.com/aasthajain25/aasthajain25.github.io/blob/main/assets/json/scatter_plot.json" text="Json Data" %}

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatter_plot.json" style="width: 100%"></vegachart>


### Description of What is Visualized:

The scatter plot visualizes data related to buildings. The x-axis represents "Square Footage," the y-axis represents "Total Floors," and the color of each point is determined by the "Building Status." Each point on the plot corresponds to a specific building and provides additional information in the tooltip, including "Agency Name," "Location Name," "Square Footage," and "Total Floors."

### Design Choices and Encoding Types:

**X-axis** : Quantitative encoding of the "Square Footage" variable on the x-axis, allowing for a continuous representation of the size of the buildings.

**Y-axis** : Quantitative encoding of the "Total Floors" variable on the y-axis, representing the number of floors in each building.

**Color** : Nominal encoding of the "Building Status" variable to determine the color of each point. Different building statuses are represented by different colors, providing a visual distinction between them.

Tooltip (tooltip encoding): Provides additional information when hovering over a data point. Displays details such as "Agency Name," "Location Name," "Square Footage," and "Total Floors," enhancing the interpretability of individual data points.

### Color Scheme:

The color scheme is determined by the "Building Status" variable, which is a nominal categorical variable. Different building statuses are represented by distinct colors to aid in visual differentiation. The specific colors assigned to each building status are determined by the default color scheme used by Altair/Vega-Lite for nominal categorical variables.

### Data Transformations:

No explicit data transformations are performed in the provided code. The scatter plot directly visualizes the raw data from the specified URL (URL_buildings), and the interactivity is implemented through selections and filtering rather than data transformations.

### Interactivity:

The scatter plot incorporates two interactive elements:

Brush Selection (brush): Users can interactively select a region in the scatter plot by clicking and dragging, creating a rectangular brush. This enables users to focus on specific subsets of data based on the selected x and y range.

Dropdown Selection (selection_state): Users can choose a specific "Building Status" from the dropdown menu. The scatter plot dynamically updates to display only the data points associated with the selected building status, allowing for focused exploration.

### Plot 2
{% include elements/button.html link="https://github.com/aasthajain25/aasthajain25.github.io/blob/main/assets/json/bar_chart.json" text="Json Data" %}

<vegachart schema-url="{{ site.baseurl }}/assets/json/bar_chart.json" style="width: 100%"></vegachart>

### Description of What is Visualized:

The bar chart visualizes the count of building entries grouped by "Usage Description." Each bar represents the count of buildings falling under different usage descriptions. The x-axis represents the count of buildings, and the y-axis represents the "Usage Description." Each bar is color-coded based on the corresponding "Usage Description," and the tooltip displays the count of buildings for each category.

### Design Choices and Encoding Types:

1. **X-axis**: The x-axis represents the count of buildings, providing a quantitative measure of the number of buildings in each category.

2. **Y-axis**: The y-axis represents the "Usage Description," a nominal categorical variable. The bars are sorted in descending order based on the count, facilitating a clear representation of the distribution of buildings across different usage descriptions.

3. **Color**: Nominal encoding of the "Usage Description" variable to determine the color of each bar. Different usage descriptions are represented by distinct colors, aiding visual differentiation.

4. **Tooltip**: The tooltip displays the count of buildings for each category, providing additional quantitative information when hovering over a bar.

### Color Scheme:

The color scheme is determined by the "Usage Description" variable, a nominal categorical variable. Each usage description category is assigned a unique color, making it easier to distinguish between different categories in the bar chart.

### Data Transformations:

No explicit data transformations are performed in the provided code. The bar chart directly visualizes the count of buildings based on the specified URL (`URL_buildings`).

### Interactivity:

The provided code does not include explicit interactivity elements such as selections or filters. It's a static representation of the count of buildings for each usage description category.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="Dataset Used" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/aasthajain25/aasthajain25.github.io/blob/main/python_notebooks/IS%20445%20-%20Homework%208.ipynb" text="Analysis" %}
</div>