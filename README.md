# ETL-Project Proposal
This repository contains all relevant code and data for our ETL project. 


* This project will contain several datasets relating zip codes in Austin to metrics we found interesting for quality of life.

* This includes: health inspection scores, parks, incident reports, etc. 

* These datasets are not necessarily related in any way other than zip codes. This would be essentially a set-up for a visualization project where we project these metrics across a physical map of Austin and see which correlate to each other. 

#ETL-Project Notes on Data

* For the restaurant inspection scores we did the following:
    * extracted the data from the Austin Data webpage at https://data.austintexas.gov/Health-and-Community-Services/Food-Establishment-Inspection-Scores/ecmv-9xxi
    * in order to create a workable set of data for the production database, the data was cleaned and filtered for relevant columns (name, score, etc.)
    * it will be loaded into a relational database
    * the final table that will be used is restaurant_scores (included in Resources)

