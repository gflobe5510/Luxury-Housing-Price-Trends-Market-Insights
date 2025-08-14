# Luxury-Housing-Price-Trends-Market-Insights
Brief Housing Price Analysis 

Dataset Overview

This project worked with two primary datasets:

luxury_homes_banded.csv

Contains detailed listings for luxury homes in King County, WA.

Key fields include:

Price, Bedrooms, Bathrooms, Sqft_Living, Year_Built

City, Zipcode, Lat, Long

Price_Band (a categorical field created by binning the Price variable into custom tiers)

luxury_bands_summary.csv

A summary table aggregated from the above dataset.

Contains Price Band, Count, Average Price, Min, Max, and other descriptive statistics by tier.

What Was Done in the Jupyter Notebook

The Python notebook (housing_mini_projects.ipynb) was used for data wrangling, feature engineering, and exploratory analysis prior to visualization in Tableau.

1. Data Cleaning and Preparation

Filtered the dataset to include only homes priced above $1M.

Removed nulls and handled potential outliers.

Created a Price_Band variable to group listings into logical luxury pricing tiers.

2. Exploratory Data Analysis (EDA)

Generated descriptive statistics on variables such as Price, Sqft_Living, Bedrooms, and Bathrooms.

Conducted outlier detection for extreme values (e.g., homes listed above $25M).

Visualized relationships between variables:

Price vs. Square Footage

Price vs. Year Built

Bedroom and Bathroom combinations vs. Price

3. Feature Engineering

Added new features such as Price_per_Sqft for deeper insights.

Used pd.cut() to categorize prices into bands for comparison in Tableau.

4. Data Export

Saved the cleaned and transformed data as luxury_homes_banded.csv.

Created an aggregated version for summary statistics in Tableau (luxury_bands_summary.csv).

What Was Done in Tableau Story

The Tableau story is titled Luxury Housing Price Trends & Market Insights and includes five key charts embedded in a narrative-style dashboard.

1. Bar Chart – Price Band Distribution

Shows the count of listings by price tier.

Reveals that the majority of homes fall into the $1.2M to $2M range.

2. Map – Price by City

Uses latitude/longitude and city-level aggregation.

Highlights that Bellevue, Medina, and Seattle have the highest concentration of luxury homes.

3. Scatterplot – Price vs. Square Footage

Plots Sqft_Living on the X-axis and Price on the Y-axis.

Bubble size reflects bedroom count; color indicates price band.

Visualizes both typical and outlier listings (e.g., ultra-luxury properties).

4. Heatmap – Bedroom/Bathroom Combinations

Rows: Bedrooms; Columns: Bathrooms.

Color: Median Price.

Helps identify which home layouts are most common and which combinations are most valuable.

5. Line Chart – Year Built vs. Median Price

Shows how home prices trend by construction year.

Color-coded by price band to examine historical price differences.

Illustrates that newer homes tend to fetch higher prices, though not uniformly.

Summary of Insights

Most luxury listings are concentrated in the $1.2M–$2M range.

High-end listings are geographically clustered in cities like Bellevue, Mercer Island, and Medina.

Square footage and price are generally correlated, but location and amenities create pricing exceptions.

The 4–5 bedroom, 4–5 bathroom layout is most common among higher-tier listings.

Newer homes generally cost more, but the price differential flattens in some tiers and years.

Conclusion

This project combines Python-based data preparation and Tableau visualization to analyze luxury real estate trends in King County, WA. The workflow includes data cleansing, exploratory analysis, price segmentation, and market insight generation. The Tableau story offers an accessible narrative for real estate professionals, analysts, or buyers seeking to understand how size, location, layout, and construction year influence pricing in the high-end market.
