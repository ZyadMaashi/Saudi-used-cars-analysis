# Which of These Factors (Brand, Mileage, Year) Are Most Linked to Used Car Prices in Saudi Arabia?

Python analysis of 5,344 Saudi used cars the listings are from Kaggle.

## Why I built this analysis
A friend of mine told me he was going to buy a used car, so the question popped up in my head, what are the most linked to factors that lower or heighten the price: year, mileage, engine size, brand and model.

## Data
The data is from the [Saudi Arabi Used Cars Dataset] (https://www.kaggle.com/datasets/turkibintalib/saudi-arabia-used-cars-dataset) on Kaggle, created by Turki Bintaleb and his collaborators, who got the listings from the Syarah website. The file I used for this analysis was the cleaned English file, which contains about 8,035 cars and 13 columns. Which is fewer than the 8,248 records on the dataset page, and I still don't know what was removed.

The data file is not included in this repository. If you wish to run the notebook download the file from Kaggle.

## What I did
1. Deleted 2,527 cars that have a price of 0 (2,526 were marked "Negotiable") and 70 cars had a mileage of 500,000 km or more.
2. Removed 94 cars that were priced under 5,000 SAR, which left me with 5,344 cars.
3. Compared median prices by each year, located a jump for the 2020-2021 models, and tested it with Toyota and the Land Cruiser.
4. Measured how prices move with year, mileage and engine size.
5. Compared brands within 2018 cars only.

## Main findings
- Brand and model looked more linked to price than year (0.32), mileage (-0.28) or engine size (0.31).
- Among the 2018 cars, the median price was ranged from 30,000 SAR (Nissan) to 214,500 SAR (Lexus).
- The 2020-2021 price increase mostly seem to come from the models that were listed and not from newer cars being worth much more.

## Limitations
- About a third of the data was removed, and I chose the 500,000 km and 5,000 SAR cutoffs myself without testing the other valus.
- I didn't look at regions or fuel types.
- These were listing prices from one website only, not final sale prices. Certain groups were small, and this shows us links, not causes.

## How to run
1. Download the data from the Kaggle link above.
2. Upload the file to the Google Colab website. The notebook expects it to be named 'UsedCarsSA_Clean_EN.csv'.
3. Run the notebook from the top.
