# Saudi Used Cars Analysis
Python analysis of 5,344 Saudi used car listings from Kaggle: how brand, year, mileage, and engine size relate to price

## Question
I wanted to find out which factors (year, mileage, engine size, brand, and model) are most strongly linked to the price of used cars in Saudi Arabia.

## Data
The data comes from the "Saudi Arabia Used Cars Dataset" on Kaggle, made by Turki Bintaleb and other collaborators, who collected the listings from the Syarah website (syarah.com). Link: [Saudi Arabia Used Cars Dataset](https://www.kaggle.com/datasets/turkibintalib/saudi-arabia-used-cars-dataset).

I used the cleaned English file from this dataset, 'UsedCarsSa_Clean_EN.csv'. it contains 8,035 cars, fewer than the 8,248 records described on the dataset page, and I don't know exactly what was removed. After my own cleaning (removing zero prices, impossible mileage, and prices under 5,000 SAR), 5,344 cars were left.

The data file isn't included in this repository, because the dataset's license says the data belongs to its original authors. To run the notebook, download the data from Kaggle and upload it to Google Colab.

## Main finding
Brand and model looked more strongly linked to used car prices than year (0.32), mileage (-0.28), or engine size (0.31). Even among 2018 cars only, Lexus's median price was about 7 times Nissan's.

## Limits
- About a third of the data was removed during cleaning (8,035 cars became 5,344), and I didn't test whether removing the "Negotiable" cars changed my results.
- These are listing prices from one website, not final sale prices.
- Many groups are small, and this shows links, not causes.

## How to run it
1. Download the data from Kaggle link above.
2. Upload the file to Google Colab. The notebook expects it to be named  UsedCarsSA_Clean_EN.csv.
3. Run the notebook from the top.

## Note on AI
I used an AI assistant throughout this project. It recommended the dataset, assisted in writing the code, and reviewed and adjusted my notes. I ran every step, checked the outputs, and made the cleaning decisions myself. 
