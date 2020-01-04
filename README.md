## big-data-challenge
Used ZEPL notebooks to ETL two datasets for Amazon reviews. Luggage and watches were analyzed and transformed to fit the given schema file using pyspark. Then the dataframes were loaded into an RDS instance using AWS.


## Data Sources
* Luggage Reviews: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Luggage_v1_00.tsv.gz
* Watches Reviews: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Watches_v1_00.tsv.gz


## Pipeline
1. Loaded data file
2. Transformations
* Dropped duplicate records
* Converted date-time to date format
* Dropped records with repeated product_id
* Filtered columns to create desired dataframes
3. Load
* schema
