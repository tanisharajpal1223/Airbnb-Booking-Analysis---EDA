# Airbnb-Booking-Analysis---EDA
Exploratory Data Analysis of Airbnb NYC 2019 data


## Project Overview
This project involves the exploration and analysis of an Airbnb dataset containing approximately 49,000 observations and 16 columns. The dataset is a mix of categorical and numeric values, and the analysis aims to uncover key insights that can aid in various business decisions. These insights can be used to enhance security, guide marketing strategies, improve customer and host experiences, and support the implementation of innovative services on the platform.

## Business Context
Since its inception in 2008, Airbnb has revolutionized the way people travel, offering unique and personalized experiences around the world. With millions of listings available globally, data analysis has become a critical tool for understanding customer and host behavior, driving business decisions, and ensuring the platform's continued growth and security.

This project focuses on analyzing Airbnb listing data to uncover trends and patterns that can inform business strategies, optimize operations, and enhance the overall experience for both guests and hosts.

## Objectives

The main objectives of this project are to:

1. Understand the key factors that influence pricing and customer behavior on Airbnb.
2. Identify popular neighborhoods and room types that are in high demand.
3. Provide actionable insights that can be used to enhance Airbnb’s marketing strategies, improve customer satisfaction, and optimize host performance.
4. Highlight any potential security concerns or risks based on the data that could hinder business growth.
5. Offer insights and recommendations to overcome obstacles impeding business growth and to enhance revenue and efficiency.

## Dataset Description

The dataset used in this project includes the following fields:

- **id**: Unique identifier for the listing
- **name**: Name of the listing
- **host_id**: Unique identifier for the host
- **host_name**: Name of the host
- **neighbourhood_group**: Location of the listing (broader area)
- **neighbourhood**: Specific area within the broader location
- **latitude**: Latitude coordinate of the listing
- **longitude**: Longitude coordinate of the listing
- **room_type**: Type of listing (e.g., entire home/apt, private room, shared room)
- **price**: Price of the listing per night
- **minimum_nights**: Minimum number of nights required for booking
- **number_of_reviews**: Total number of reviews received by the listing
- **last_review**: Date of the last review

## Libraries Used
The following Python libraries are used for data analysis and visualization:

- **Pandas**: For data manipulation, aggregation, and cleaning.
- **NumPy**: For efficient numerical operations and calculations.
- **Matplotlib**: For creating static visualizations of the data.
- **Seaborn**: For creating more advanced and aesthetically pleasing visualizations.

## Methodology

### Data Wrangling

1. **Handling Missing Values**
   - Replaced missing values with `NaN` values.

2. **Dropping Null Values**
   - Dropped all null values from the following columns: `name`, `host_name`, `last_review`, and `reviews_per_month`.

3. **Data Type Conversion**
   - Converted the data types of the following columns to `float`: `price`, `minimum_nights`, `number_of_reviews`, `calculated_host_listings_count`, `availability_365`.
   - Converted the `last_review` column to a `datetime` object.

4. **Removing Duplicates**
   - Dropped duplicate values from the dataset.

5. **Outlier Detection and Removal**
   - Detected outliers in the `price` column using boxplots and removed them.

6. **Data Insights After Wrangling**
   - The `neighbourhood_group` column has the following distribution:
     - Manhattan: 15,071 values
     - Brooklyn: 15,107 values
     - Queens: 4,148 values
     - Bronx: 733 values
     - Staten Island: 266 values
   - The `room_type` column has the following distribution:
     - Entire home/apt: 18,526 values
     - Private room: 16,304 values
     - Shared room: 495 values

7. **Final Dataset**
   - After data wrangling, the data frame now contains 35,325 rows and 16 columns.


## Analysis and Visualizations
The project includes a thorough exploratory data analysis (EDA) to identify patterns, trends, and outliers within the dataset. At least five different types of visualizations are used to understand the distribution of data, correlations between variables, and behavior concerning the target variable (e.g., price or number of reviews). These visualizations may include:

- **Histograms**: To understand the distribution of continuous variables like price and minimum nights.
- **Bar Charts**: To analyze categorical data, such as room type and neighborhood.
- **Scatter Plots**: To explore relationships between numerical variables, like price and number of reviews.
- **Heatmaps**: To visualize correlations between multiple variables.
- **Box Plots**: To identify outliers and understand the spread of data.

## Recommendations and Actionables

Based on our data analysis, we recommend the following strategies to achieve the business objectives:

1. **Expand Listing Across Neighborhoods**
   - Our analysis reveals that the majority of `calculated_host_listings_count` are concentrated in Manhattan, while other neighborhood groups have significantly lower counts. To diversify and capitalize on high-demand areas, we suggest hosts consider listing their properties in other popular neighborhoods. For example, Brooklyn is highly demanded and popular, making it a promising area for property listings.

2. **Enhance Private and Shared Room Offerings**
   - The data shows that the `Entire home/apt` room type is significantly more popular compared to private and shared rooms. To increase overall revenue, we recommend improving the facilities and guest experience for private and shared room types. This enhancement could attract more bookings and balance the revenue across different room types.

3. **Increase Availability of Entire Home/Apt**
   - The availability of `Entire home/apt` rooms is notably lower than other room types. Increasing the number of available properties in this category could lead to positive business growth and higher revenue. Expanding the inventory of `Entire home/apt` listings might better meet customer demand and improve market share.


## Conclusion

Throughout this data science project, we conducted extensive exploratory data analysis (EDA) to uncover valuable insights and patterns within the dataset. This process not only honed our critical thinking skills but also enabled us to extract actionable information from the data.

We utilized various data visualization techniques, including bar graphs, box plots, scatter plots, and histograms, to analyze the dataset. Bar graphs were instrumental in examining relationships between categorical and continuous variables. Box plots allowed us to detect and address outliers, while scatter plots provided clarity on the relationships between continuous variables. Histograms were useful for understanding the distribution of these variables.

The insights gained from these analyses are expected to significantly benefit the business by informing strategic decisions and fostering positive growth. By leveraging these findings, the business can enhance its operations, optimize performance, and drive greater success.



