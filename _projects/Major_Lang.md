---
name: Language Family Distribution and Vulnerabilities
tools: [Python, HTML, vega-lite]
image: assets/pngs/langmap.png
description: This is a distribution to see how language families are distributed and their vulnerabilities to extinction.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Major language family distribution
## Created by: Aastha and Utsav
<br>

A visualization that represents how major world language families are distributed. 
The interactive chart provides insight on how vulnerable the languages are within a family.
The networks provide an insight on how simialr the languages are and how they can be subcategorized into communities.
At the bottom of the page, I have provided the data and the code for further analysis.
If the code is forked, it can be used for more dynamic interactivity in Jupyter notebook using widgets.

We have selected 5 language families (Indo-European, Afro-Asiatic, Atlantic-Congo, Austronesian, and Sino-Tibetan) for our visualizations. For each family group, we have 2 dashboards. The first one contains two interactive visualizations: a bar chart displaying the distribution of languages by their endangerment status within the selected family, and a heatmap illustrating the distribution of languages within sub-families. The bar chart allows users to brush over specific status categories, dynamically updating the heatmap. Additionally, the dashboard includes a geographical plot on a world map, marking the locations of languages from the subset of the dataset for the language family. Each language is color-coded based on its endangerment status. The resulting visualizations provide a comprehensive overview of language distribution, status, and geographic locations within the selected language family.

The second dashboard features two visualizations of a language similarity network. The first plot depicts the network graph, where nodes represent languages and edges signify similarities between them. The size and color of nodes are determined by the cumulative similarity with neighboring languages, and the edge widths indicate the strength of similarity. The color bar on the side represents the range of node colors, corresponding to the sum of similarities. The second plot focuses on community detection within the network, revealing distinct groups of languages with shared similarities. Both visualizations provide insights into the structure and relationships within the language subset, highlighting patterns of similarity and community organization.

<br>

### Indo-European

Map
![Indo-European](/assets/pngs/Finals/Indo-European.png)
Interactive Chart
<vegachart schema-url="{{ site.baseurl }}/assets/json/Finals/Indo-European.json" style="width: 100%"></vegachart>
Similarity Network on 20 random languages
![Indo-European](/assets/pngs/Finals/Networks/Indo-European_main_network.png)
![Indo-European](/assets/pngs/Finals/Networks/Indo-European_community_detection.png)

<br>

### Afro-Asiatic

Map
![Afro-Asiatic](/assets/pngs/Finals/Afro-Asiatic.png)
Interactive Chart
<vegachart schema-url="{{ site.baseurl }}/assets/json/Finals/Afro-Asiatic.json" style="width: 100%"></vegachart>
Similarity Network on 20 random languages
![Afro-Asiatic](/assets/pngs/Finals/Networks/Afro-Asiatic_main_network.png)
![Afro-Asiatic](/assets/pngs/Finals/Networks/Afro-Asiatic_community_detection.png)

<br>

### Atlantic-Congo

Map
![Atlantic-Congo](/assets/pngs/Finals/Atlantic-Congo.png)
Interactive Chart
<vegachart schema-url="{{ site.baseurl }}/assets/json/Finals/Atlantic-Congo.json" style="width: 100%"></vegachart>
Similarity Network on 20 random languages
![Atlantic-Congo](/assets/pngs/Finals/Networks/Atlantic-Congo_main_network.png)
![Atlantic-Congo](/assets/pngs/Finals/Networks/Atlantic-Congo_community_detection.png)

<br>

### Austronesian

Map
![Austronesian](/assets/pngs/Finals/Austronesian.png)
Interactive Chart
<vegachart schema-url="{{ site.baseurl }}/assets/json/Finals/Austronesian.json" style="width: 100%"></vegachart>
Similarity Network on 20 random languages
![Austronesian](/assets/pngs/Finals/Networks/Austronesian_main_network.png)
![Austronesian](/assets/pngs/Finals/Networks/Austronesian_community_detection.png)

<br>

### Sino-Tibetan

Map
![Sino-Tibetan](/assets/pngs/Finals/Sino-Tibetan.png)
Interactive Chart
<vegachart schema-url="{{ site.baseurl }}/assets/json/Finals/Sino-Tibetan.json" style="width: 100%"></vegachart>
Similarity Network on 20 random languages
![Sino-Tibetan](/assets/pngs/Finals/Networks/Sino-Tibetan_main_network.png)
![Sino-Tibetan](/assets/pngs/Finals/Networks/Sino-Tibetan_community_detection.png)

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/aasthajain25/aasthajain25.github.io/blob/main/python_notebooks/Language_viz_revised.ipynb" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/utsavm2/Language_Visualization/blob/main/Final_Project/Code/Language_viz_revised.ipynb" text="The Analysis" %}
</div>
