# Tokopedia Web Scraping

This repository is an automated web scraping method, to scrape or collect data from a famous e-commerce in Indonesia, Tokopedia. The scrape method is build using Python language, with the help of Python's library:
 - **Selenium** to automate the scraping process,
 - **Beautiful Soup** to scrape the data from the website, and
 - **Pandas** to transform the data into DataFrame and save it to csv format.

(**Note** : The program is build using Python version >=3.8 and the browser that I'm using is Chrome version 10.)

## Steps
1. Create the conda environment:
    ```
    conda env create --file=tokped_scraper.yml
    ```
2. Activate the conda environment:
   ```
   conda activate tokped_scraper.yml
   ```
3. Change the variables (see **Changeable Variables** below)
4. Run `scraper.py`:
   ```
   python scraper.py
   ```

## Changeable Variables
Here is the variables that you can change to your preference:
|Variable Name       |Line |Definition                                        |                          
|--------------------|-----|--------------------------------------------------|
|Browser driver path |16   |The path to your browser's driver                 |
|url                 |19   |Tokopedia's url page that you want to scrape      |
|page                |30   |Range of pages that you want to scrape            |
|dataset.csv         |97   |Path for the scraping result, saves in .csv format|

## Web scraping result
Here is the list of column name and definition in `dataset.csv` file:
|Column Name|Definition                                         |                          
|-----------|---------------------------------------------------|
|Penjual    |Seller name/shop                                   |
|Lokasi     |City or state of the shop/seller                   |
|Produk     |Name of the product                                |
|Harga      |Price of the product (in IDR)                      |
|Rate       |The overall rating of the product                  |
|Terjual    |Estimation number of sold items for a given product|


## References:

- https://www.youtube.com/watch?v=iwC8Sv6_Am0&ab_channel=IKeepOnTrack
- https://medium.com/@yohan.ardiansyah90/web-scraping-with-python-in-indonesian-e-commerce-tokopedia-part-1-getting-the-data-a338ebd56306