# VISUAL EXPLORATION OF LARGE EARTH SURFACE TEMPERATURE, CARBON EMISSIONS AND SEA LEVEL DATASETS

## INTRODUCTION
Our system strives to solve the problem of visualizing the complex and large datasets related to earth's climate. Through a combination of data visualization, mapping, and interactive features, our interface intends to provide a unique and engaging way to explore the impacts of climate change on our planet. We have mainly focused on three datasets:
+ [Climate Change: Earth Surface Temperature Data](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data)
+ [Carbon Dioxide Emissions of the World (1990-2018)](https://www.kaggle.com/datasets/ankanhore545/carbon-dioxide-emissions-of-the-world)
+ [Global Sea Level Rise](https://www.kaggle.com/datasets/jarredpriester/global-sea-level-rise)

## Tasks
Data Pre-Processing: Data pre-processing refers to the process of prepar-
ing data for analysis by cleaning, transforming, and reducing the raw data into a more
manageable format. It is a crucial step in data analysis, as the quality of the output
depends largely on the quality of the input data.<br>

We performed data pre-processing by following several steps:
+ Data Cleaning: This step involves removing irrelevant, duplicate, or inconsistent
data, dealing with missing data, and correcting data errors and inconsistencies.
  +  Missing values: We handled missing values in our data in an efficient manner.
For example, in temperature dataset, there were quite a few missing data for
some cities. In order to handle this scenario, we averaged the data of its
neighboring cities and filled in the values.
  + Irrelevant features: We removed certain columns that were not useful for cre-
ating meaningful visualization.
+ Data Transformation: This step involves converting data into a more meaning-
ful format, such as normalizing data, transforming categorical data into numerical
data, or applying mathematical operations to data.

+ Data Analysis: This step refers to the process of systematically examining and
interpreting data with the goal of extracting useful information and insights. It
involves using various statistical and computational methods to identify patterns,
relationships, and trends within a dataset.
   + We analysed the attributes of our datasets and came up with the best suitable
visualization for it.


## Proposed Solution
We propose a standalone interface, built entirely from scratch
using the Plotly Dash. It is a Python framework for building web applications that are
focused on data visualization and analysis.

## Libraries Used
+ Plotly: Plotly provides a range of interactive visualization options that allow users
to explore and analyze their data in real-time. These visualizations can be cus-
tomized with various parameters and settings, and can be easily linked to data
sources. We created several visualizations using the Plotly library, some of them
being, Choropleth Maps, Heat Maps, Bar Charts, Line Charts, Box & Whiskers
Plot, Area Chart, Map Boxes, Globes, Bubble Plots and more. The entire descrip-
tion of all the visualizations will be given in the next paragraph.
+ Pandas: Pandas is a Python library for data manipulation and analysis. It provides
a range of functions and tools for working with structured data, including data
frames and series. We used Pandas for loading and manipulating our the original
datasets as per our requirements.
+ Numpy: NumPy is a Python library for numerical computing that provides pow-
erful array manipulation and mathematical operations. It is a fundamental library
for scientific computing in Python, providing support for mathematical operations
on large, multi-dimensional arrays and matrices. We used Numpy for applying
tranformations on our datasets.
+ Json: JSON stands for JavaScript Object Notation, and it is a lightweight data
interchange format that is easy to read and write. It is based on a subset of the
JavaScript programming language and is often used to transmit data between a
server and a web application, as an alternative to XML. In order to read and load
the GeoJson files for creating visulaizations of mapbox in the temperature datsets,
Json is used.
+ Matplotlib: Matplotlib is a Python library for creating visualizations of data. It
provides a range of functions and tools for creating a wide variety of plots and
charts, including line plots, scatter plots, histograms, and more. We created a few
visualizations of bar chart and line chart with the help of Matplotlib.

## Results
We created a standalone interface visualizing the changes in Earth’s surface temperature,
carbon emissions and sea levels over the years.

+ Homepage
<img width="800" alt="Screenshot 2023-04-24 at 12 12 23" src="https://user-images.githubusercontent.com/100257642/234190921-b12c524a-8b37-45ad-924c-e12df7c7de6a.png">

+ Visualization: Temperature
  + Calendar Heat Map
  <img width="800" alt="Calender Heat Map" src="https://user-images.githubusercontent.com/100257642/234192422-e262268f-765b-46bb-ada1-0a83eafcda99.png">

  + Choropleth Map
  <img width="800" alt="Choropleth_temp" src="https://user-images.githubusercontent.com/100257642/234192533-448c7877-e7e4-4337-92ac-26ba63f88550.png">

  + Earth Temperature Timeline
  <img width="800" alt="Earth Temp Timeline" src="https://user-images.githubusercontent.com/100257642/234192552-898bb64e-54a5-497c-8302-f39f4ebfe0b9.png">

  + 3-D Globe Representation
  <img width="800" alt="Globe_3d" src="https://user-images.githubusercontent.com/100257642/234192561-2d3ac8ee-4698-4121-bc3c-7fe117971446.png">

  + Heat Map
  <img width="800" alt="Heatmap_temp" src="https://user-images.githubusercontent.com/100257642/234192580-572f03cf-a785-41de-b953-3c87371b5deb.png">

  + Map Box
  <img width="800" alt="Mapbox-India" src="https://user-images.githubusercontent.com/100257642/234192602-1092f392-49dd-4c32-8cda-1b7f63cf4ec4.png">
  <img width="800" alt="Mapbox-China" src="https://user-images.githubusercontent.com/100257642/234192618-29deec29-c185-4b13-bab9-5c076caf0759.png">
  <img width="800" alt="Mapbox-Canada" src="https://user-images.githubusercontent.com/100257642/234192642-9cad8871-7a70-4b10-92fb-02000b8094dc.png">
  <img width="800" alt="Mapbox-Brazil" src="https://user-images.githubusercontent.com/100257642/234192658-f652d75c-209d-4b9d-b88c-c7395efc1aa9.png">
  <img width="800" alt="Mapbox-Russia" src="https://user-images.githubusercontent.com/100257642/234192678-07a60b9f-8b5d-4dd0-bf82-f29c04e53de6.png">
  <img width="800" alt="Mapbox-USA" src="https://user-images.githubusercontent.com/100257642/234192695-7f8e4d44-1bb5-48c8-9c63-e3c87b27b11d.png">

  + Line Charts
  <img width="800" alt="Line Chart- Continents" src="https://user-images.githubusercontent.com/100257642/234192710-d58d3cc5-d7ff-45d7-9feb-0507a10b8736.png">

  + Globe-2D
  <img width="800" alt="Globe-2d Difference" src="https://user-images.githubusercontent.com/100257642/234192729-a973ef39-3a9b-4e15-930d-f3244a08d37f.png">

  + Difference Bar Chart
  <img width="800" alt="Bar Chart-Difference" src="https://user-images.githubusercontent.com/100257642/234192758-8c5d0274-c753-49e5-b201-26f627d5d881.png">

  
+ Carbon Emissions

  + Scatter Plot
  <img width="800" alt="Scatterplot_CO2" src="https://user-images.githubusercontent.com/100257642/234192814-0ae253a1-4ff3-4375-9a94-750fadbfc6c2.png">

  + Bar Chart Race
  <img width="800" alt="BarChart_Race" src="https://user-images.githubusercontent.com/100257642/234192824-d00e327a-ea36-415c-8547-400089b13eb0.png">

  + Bar Chart
  <img width="800" alt="BarChartCO2_Top5" src="https://user-images.githubusercontent.com/100257642/234192869-fc969b45-ab71-4fdd-ba19-29e2ca1a5b1f.png">
  <img width="800" alt="BarChartCO2_Bottom5" src="https://user-images.githubusercontent.com/100257642/234192887-59744860-03d4-465f-b542-605065ea6d90.png">

  + Bubble Plot
  <img width="800" alt="Bubbleplot" src="https://user-images.githubusercontent.com/100257642/234192904-dfbed3a5-30f3-476a-9bd6-62f88da5a49e.png">

  
  + Line Chart
  <img width="800" alt="LineChartCO2_Top5" src="https://user-images.githubusercontent.com/100257642/234192928-7b20199d-6297-4c77-84b4-105a3f5ab0da.png">
  <img width="800" alt="LineChartCO2_Bottom5" src="https://user-images.githubusercontent.com/100257642/234192939-331671d5-95e9-40d5-9679-c8c342072750.png">

  + Choropleth Map
  <img width="800" alt="ChoroplethCO2_Choro" src="https://user-images.githubusercontent.com/100257642/234192948-74e2b7c2-31cc-4ddf-ba35-b6cf960f2bbe.png">

  + Heat Map
  <img width="800" alt="HeatmapCO2" src="https://user-images.githubusercontent.com/100257642/234192961-4c3889ad-2182-4917-a58f-1bef2601c2d9.png">

+ Sea Level
   + Bar Chart
   <img width="1800" alt="SeaLevel_Bar" src="https://user-images.githubusercontent.com/100257642/234192982-79488041-0032-457f-977b-769001cf2012.png">

   + Scatter Plot
   <img width="800" alt="SeaLevel_Scatterplot" src="https://user-images.githubusercontent.com/100257642/234192991-97fe869c-2f77-4c73-a4e3-7719b04a4245.png">

   + Box and Whiskers Plot
   <img width="800" alt="SeaLevel_Box1" src="https://user-images.githubusercontent.com/100257642/234193003-0d482a05-1216-4754-8280-d14fe40c9334.png">
   <img width="800" alt="SeaLevel_Box2" src="https://user-images.githubusercontent.com/100257642/234193016-e69023d0-c0bc-455f-b7ae-eb2f9566f331.png">

   + Area Chart
   <img width="800" alt="SeaLevel_Area" src="https://user-images.githubusercontent.com/100257642/234193033-8fe7bfb3-8c12-4204-8223-e460f13bb245.png">

   + Line Chart
  <img width="800" alt="SeaLevel_line" src="https://user-images.githubusercontent.com/100257642/234193062-e0aff12b-2333-436d-a57c-ea4008f671dd.png">


+ Correlation 
  + Stacked Bar Chart
  <img width="800" alt="corr1" src="https://user-images.githubusercontent.com/100257642/234193415-22f34039-7a75-4353-bd29-1abbfec7dc16.png">
  <img width="800" alt="corr3" src="https://user-images.githubusercontent.com/100257642/234193512-aa1b3ddc-22c0-4a30-a9fb-6c6e99cafc25.png">

  + Line Chart
  <img width="800" alt="corr2" src="https://user-images.githubusercontent.com/100257642/234193496-24f2167c-df26-4188-8100-dcfa6abfb1a2.png">
  <img width="800" alt="corr4" src="https://user-images.githubusercontent.com/100257642/234193524-b77a3969-250a-450d-9270-4f2f0b7d42c1.png">

  + Scatter Plot
  <img width="800" alt="corr5" src="https://user-images.githubusercontent.com/100257642/234193549-7c157639-1909-47ea-bb23-d939756238b2.png">













