# Housing Rental

## Analysis for San Francisco

Using data visualization skills, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

The main task is to visualize and analyze the real-estate data in Jupyter notebook. Completed the following tasks using the san_francisco_housing.ipynb:

- Calculated and plotted the housing units per year.

- Calculated and plotted the average prices per square foot.

- Compared the average prices by neighborhood.

- Built an interactive neighborhood map.

- Composed data story.

Calculated and Plotted the Housing Units per Year
using and visual aggregation to calculate the number of housing units per year, and then visualize the results as a bar chart. To do so, complete the following steps:

Grouped the data by year. Aggregated the results by the mean of the groups.

Used the hvplot function to plot the housing_units_by_year DataFrame as a bar chart. Made the x-axis represent the year and the y-axis represent the housing_units.

Styled and formatted the line plot to ensure a professionally styled visualization.

Note that your resulting plot should appear similar to the following image:

Answered the Following:

- What’s the overall trend in housing units over the period that you’re analyzing?

Calculated and Plotted the Average Sale Prices per Square Foot
using numerical and visual aggregation to calculated the average prices per square foot, and then visualized the results as a bar chart. Completed the following steps:

- Grouped the data by year, and then averaged the results. 
- Noted lowest gross rent.

Created a new DataFrame named prices_square_foot_by_year by filtering out the “housing_units” column. 

Used hvPlot to plot the prices_square_foot_by_year DataFrame as a line plot.

Styled and formatted the line plot to ensure a professionally styled visualization.

Used both the prices_square_foot_by_year DataFrame and interactive plots to answer the following questions:

- Did any year experience a drop in the average sale price per square foot compared to the previous year?

- If so, did the gross rent increase or decrease during that year?

# Compared the Average Sale Prices by Neighborhood
Completed the following steps:

- Created a new DataFrame that groups the original DataFrame by year and neighborhood. Aggregated the results by the mean of the groups.

- Filtered out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.

- Created an interactive line plot with hvPlot that visualizes both sale_price_sqr_foot and gross_rent. Set the x-axis parameter to the year (x="year"). Used the groupby parameter to create an interactive widget for neighborhood.

Styled and formatted the line plot to ensure a professionally styled visualization.

Used the interactive visualization to answer the following question:

- For the Anza Vista neighborhood, is the average sale price per square foot for 2016 more or less than the price that’s listed for 2012?
# Built an Interactive Neighborhood Map
Completed the following steps:

Read the neighborhood_coordinates.csv file from the Resources folder into the notebook, and create a DataFrame named neighborhood_locations_df. Set the index_col of the DataFrame as “Neighborhood”.

Using the original sfo_data_df Dataframe, created a DataFrame named all_neighborhood_info_df that groups the data by neighborhood. Aggregated the results by the mean of the group.

Using hvPlot with GeoViews enabled, create a points plot for the all_neighborhoods_df DataFrame. Be sure to do the following:

- Set the geo parameter to True.
- Set the size parameter to “sale_price_sqr_foot”.
- Set the color parameter to “gross_rent”.
- Set the frame_width parameter to 700.
- Set the frame_height parameter to 500.
- Include a descriptive title.

Use the interactive map to answer the following question:

- Which neighborhood has the highest gross rent, and which has the highest sale price per square foot?

# Compose Data Story

- How does the trend in rental income growth compare to the trend in sales prices? Does this same trend hold true for all the neighborhoods across San Francisco?

- What insights can you share with your company about the potential one-click, buy-and-rent strategy that they're pursuing? Do neighborhoods exist that you would suggest for investment, and why?