# Taobao-TMALL Items-Data Extractor
A script for extracting items info from Taobao-TMALL shops(淘宝天猫旗舰店). 

# Definition of Nouns
+ **items category page**: the "item by sales" page from each shop. Similar to the following page:
  ![item category page](./img/example_item_by_sales_page.jpg)

# Features:
1. [tools/theDataExtractor.js](./tools/theDataExtractor.js): Extract the info of the top 15 items, then parse and download the following files:
  + a csv File, contains all text info.
  + item thumbnails.

2. [src/index.ts](./src/index.ts):
  + open tabs, to the homepage of the shops, 
Open home-pages of shops in new browser tabs. You can then maually goes to any [items category page](#Definition of Nouns), then use theDataExtractor.


# Usage:
## Extract Items Infomation From TMALL shops
   + paste the [tools/theDataExtractor.js](./tools/theDataExtractor.js) in the console of an **item category page** of a **TMALL shop**, as shown here, then hit the Enter key to run:
   ![basic usage](./img/example_usage.png)

## (Alternative) Auto Open TMALL Shops by "shopName" in Browser Tabs
+ (modify the "shopNames" parameter in [tools/puppeteerStealthPoC.ts](./tools/puppeteerStealthPoC.ts))
+ After installing node.js and npm install intially:
  1. npm run dev.
  2. When the Taobao main page loads, login and wait.

# Result Example
+ csv content:
  ![item data in csv](./img/example_csv.jpg)
  
+ data downloaded(csv + thumbnails):
  ![item data and thumbnails](./img/example_dowloaded_data.jpg)

