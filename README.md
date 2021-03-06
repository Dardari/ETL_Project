#ETL-Project Final Notes

    * For the datasets used, we took csv files from several sources. From the Austin Data page at data.austintexas.gov, we files for parks, restaurant inspection scores, crime incidents, etc. The datasets had to include zip codes, so that we could aggregate all of our indicators of quality of life and group them together by zip code. Basically, we were trying to measure quality of life through numbers and metrics for Austin Zip Codes and compare them to each other.
            
            *example datasets:
               1. https://data.austintexas.gov/Health-and-Community-Services/Food-Establishment-Inspection-Scores/ecmv-9xxi
               2. https://www.kaggle.com/jboysen/austin-crime#austin_crime.csv
    * We downloaded our datasets, cleaned them of any irrelevant columns and dropped duplicates, forming dataframes. After exporting these dataframes into SQL workbench tables, we then developed one final aggregate table to show all quality of life metrics.
    
    * We used SQL workbench because it is much more intuitive for the type of project we want. As far as joining tables and doing subqueries, it was easier for us to use.

    * Potential analysis on the dataset we created could be inquiries such as:

        *   What zip codes have the cleanest restaurants on average?
        *   What zip codes see more crime vs. others?
        *   What zip codes have the most parks?
    *   We faced a few challenges along the way. From a logistical view, exporting data into a SQL workbench is very finnicky and you can run into errors such as index conflicts. Once this is done, we have to deal with the structure of our datasets being different. For example, the parks dataset can be significantly smaller than the restaurant inspection dataset. So we not only need to group the averages of inspection scores but also figure out a subquery to accurately join the two tables and display correct metrics. 

