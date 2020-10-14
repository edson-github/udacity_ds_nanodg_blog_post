# DS Nanodegree Project: Write a Data Science Blog Post
## Description
The goal of writing a data science blog post is two make use of the CRISP-DM methodology.
CRISP-DM stands for cross industry standard process for data mining. The main steps components are:
* Business Understanding
* Data Understanding
* Data Preparation
* Modeling
* Evaluation
* Deployment

For the blog post I've decided to analyze and answer questions related to the [Olist marketplace datasets](https://www.kaggle.com/olistbr/brazilian-ecommerce) found in Kaggle. The questions are the following:

1. Which product categories contribute the most to total products purchased?
2. From which cities are most products being bought from?
3. Is there any seasonality to the number of orders placed?

The exploratory data analysis that led to these questions, and their respective answers are found in `eda.ipynb` under the `olist_ecommerce_eda` directory. No modelling or predictive analytics was done so the last three steps of CRISP-DM will not be relevant. Below a brief decription of all relevant directories and files.

## Directories and Files
```
.
|-- README.md
|-- environment.yml
|-- olist_ecommerce_eda
|   |-- eda.ipynb
|   |-- graphs_tables
|   |   |-- city_product_count_summary_statistics_table.png
|   |   |-- city_products_count_cdf.png
|   |   |-- daily_orders_autocorrelation_plot.png
|   |   |-- dfuller_pvals_table.png
|   |   |-- monthly_products_plot.png
|   |   |-- orders_daily_plot.png
|   |   |-- top10_categories_monthly_share_products_heatmap.png
|   |   |-- top10_cities_monthly_share_products_heatmap.png
|   |   |-- top10_cities_products_table.png
|   |   |-- top10_product_categories_products_table.png
|   |   `-- weekday_orders_plot.png
|   |-- olist_customers_dataset.csv
|   |-- olist_order_items_dataset.csv
|   |-- olist_orders_dataset.csv
|   |-- olist_products_dataset.csv
|   |-- olist_sellers_dataset.csv
|   `-- product_category_name_translation.csv
`-- tsa_olist.md

```

* `olist_ecommerce_eda/eda.ipynb`: exploratory data analysis, covers business understanding, data understanding and data preparation from CRISP-DM methdology
* `olist_ecommerce_eda/graphs_tables`: PNG files of graphs and tables used for the blog post.
* `tsa_olist.md`: local markdown blog post, similar will be published in medium.
* `environment.yml`: conda environment files with all dependencies, see Environment section for replication. 

## Medium Blog Post
Can be found [here](medium link) # TODO

## Environment
For those working with conda, you can find the full environment in the `environment.yml` file, the name is `py37_ml` 
* To replicate, run `conda env create -f environment.yml`
* To activate, run `conda activate py37_ml`

If you're using any other environment management system, the following are the main packages to install, latest versions should work:

```
pandas
numpy
statsmodels
matplotlib
seaborn
fbprophet
dataframe_image
holidays
```

## Opening the Notebook
Run the following in the terminal `jupyter notebook ` or `jupyter lab` if you have it installed.

## Acknowledgements
Thanks to [Olist](https://olist.com) for making the datasets available in [Kaggle](https://kaggle.com/).