# Amazon Vine Analysis

## Overview
Using US Apparel product reviews from Amazon, the goal was to analyze if it would be beneficial to subscribe to a Vine program if we were to sell similar products through their platform. The vine review program is an incentive model in which customers are gifted free products when they submit good reviews. We used PySpark to extract, transform, and load (ETL) the data to a AWS RDS that was created and connected to a PostgreSQL server allowing the ability to  query and extract the tables of data needed to perform an analysis.

## Deliverable 1
The first step in the process was to extract the data from the Apparel dataset and create a dataframe within Google Collab Notebook.

![Screen Shot 2022-03-15 at 8 20 09 PM](https://user-images.githubusercontent.com/93485455/159191297-2c644fa2-1d40-466c-83d0-f86a4243ff11.png)

Then we took the data and broke into four different dataframes

![Screen Shot 2022-03-15 at 8 20 28 PM](https://user-images.githubusercontent.com/93485455/159191363-920cdd47-0040-4357-aae7-9b6daafc421c.png)

![Screen Shot 2022-03-15 at 8 20 38 PM](https://user-images.githubusercontent.com/93485455/159191369-512a9f28-aa77-40df-b1d6-ed0a17903fd9.png)

![Screen Shot 2022-03-15 at 8 20 48 PM](https://user-images.githubusercontent.com/93485455/159191378-954afe47-fc61-4b3d-a984-349cbdef5e7e.png)

![Screen Shot 2022-03-15 at 8 20 57 PM](https://user-images.githubusercontent.com/93485455/159191382-4badcae7-1220-4304-b8d4-661df2063274.png)

With use of AWS datacloud, transferred the data into a postgres DB locally.

![Screen Shot 2022-03-15 at 8 45 09 PM](https://user-images.githubusercontent.com/93485455/159191417-081fc4a2-26af-4455-84e1-99627f5ad6c7.png)

![Screen Shot 2022-03-15 at 8 47 47 PM](https://user-images.githubusercontent.com/93485455/159191436-fb0d9e27-1b84-47a4-869a-20ac7f1acc5f.png)

![Screen Shot 2022-03-15 at 8 57 53 PM](https://user-images.githubusercontent.com/93485455/159191453-f771ddc5-58da-4161-81dc-f42b4fb842f0.png)

![Screen Shot 2022-03-15 at 9 21 47 PM](https://user-images.githubusercontent.com/93485455/159191460-dbc4170c-4df8-4468-8345-dfc2fc8535f3.png)

Lastly we exported the Vine table data out as a csv file to import into Juypter Notebook.


## Deliverable 2

### Paid Vine Program

33 total reviews
15 5-star reviews
45.5% of vine reviews were 5-star
Unpaid reviews

45,388 total reviews
23,733 5-star reviews
52.3% of unpaid reviews were 5-star

## Deliverable 3

While the percentages of five star reviews appear to be similar, the volume of the non paid Vine program is much larger than paid subscribers. Based on these results it allows the conclusion that customers who are part of the paid program do not feel a positive bias leaving good reviews. Even though there is a slight 0.2 difference in the average review-star rating in favor of the Vine program it does not seem as popular in this product category. Further analysis by executing an NLP sentiment analysis could give insight on key words used in reviews to determine if the Vine reviews were more detailed and effusive in praise of the products.
