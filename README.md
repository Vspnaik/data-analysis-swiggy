# Restaurant Data Analysis for Swiggy

This is an analysis of the restaurant data on Swiggy made with Python. It summarizes various restaurants by their rating, price range, types of cuisine, and areas. The key points will include the most important distributions as well as visualizations describing the restaurant landscape.

## Goals
Preprocessing: Cleaning of the data ready for analysis.
- Analyze rating of restaurants, price and cuisine.
- Plot your insights with multiple plot generation techniques.
- Geospatial analysis of restaurant locations distribution.

## Dependencies
 `pandas` for the data manipulation and analysis purpose.
 `numpy` to perform any numerical operations
 `matplotlib` and `seaborn` are used to plot data points.
 `plotly` for the interactive plots generation.
 `geopy` for geospatial location mapping.
 `wordcloud` for the word clouds generation for cuisine data
 `kaggle` for the dataset download process.

You can install the necessary packages by running:
 
```bash
pip install pandas numpy matplotlib seaborn plotly geopy wordcloud kaggle
```
 
## Dataset
- The dataset for this analysis is the Swiggy Restaurants dataset available on Kaggle.
- This dataset consists of the following information related to restaurants:
  - Restaurant Name
  - Average Price
  - Rating
  - Number of Ratings
  - Cuisine Type
  - Location
  - Offer Name
  
### Downloading the Dataset:
```bash
!kaggle datasets download rrkcoder/swiggy-restaurants-dataset
```
### Analysis Overview
1. **Data Preprocessing**
   Cleaned the dataset by dealing with missing values and transforming columns like ratings and number of ratings into numerical types.
   Categorized restaurants based on the vegetarian status and transformed rating data into categorical bins.

2. **Price and Rating Distribution:**
-Analysed the distribution of restaurant ratings and average price across categories by using pie charts and scatter plots.

3. **Cuisine Analysis:**
Extracted and represented the most common cuisines offered by the restaurants along with the frequency distributions via word clouds and bar charts.

4. **Geospatial Analysis:**
Utilized `geopy` to extract location coordinates of restaurants and plotted them on a map.
- Generated heatmaps to illustrate the density of restaurants across various regions.

## Visualizations
- **Pure Veg Restaurants**: A pie chart representing the percentage of pure veg restaurants.
- **Rating Distribution**: A pie chart that represents restaurant ratings, split into buckets (0-3, 3-4, 4+).
- **Price Range Distribution**: A pie chart that illustrates restaurant price range distribution.
- **Top 15 Cuisines**: A bar chart that represents the top 15 cuisines among the restaurants.
- **Geospatial Maps**:
  - A scatter map of restaurant locations in India.
  - A density heatmap to represent restaurant concentration in various regions.

## How to Run
1. Download the dataset from Kaggle and extract the contents into your working directory.
2. Run the code in a Jupyter Notebook or Python script environment to perform the analysis and visualize the results.

## Conclusion
This analysis provides a comprehensive understanding of the Swiggy restaurant dataset, including trends in restaurant pricing, ratings, and cuisine types. Geospatial visualizations offer insights into the distribution of restaurants across various locations.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
