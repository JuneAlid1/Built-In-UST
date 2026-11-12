
# IN CURSOR
# Crop picker chat summary

Work in this chat was on the OPMT 375 storefront, mainly `mn-crop-picker.html` and the home page.

## Home page link

The storefront home page (`index.html`) has a **Crop picker** section. It links to `mn-crop-picker.html` with the text “Which crop should we add next?”

## Download link

The crop picker footer says **Download new data from here** and links to the USDA NASS Quick Stats query for Minnesota crop production value: survey data, state level, annual, dollars, from 2015 on, as CSV.

## Nothing shown until a file is loaded

Top picks, the ranking chart, the trend chart, and the full table stay hidden until a dataset loads. Before that, the page shows the question, the file picker, and the download link. A missing file does not show an error.

## Total rows left out

Rows whose crop name contains “total” are left out of the picks, the ranking chart, and the table. That removes aggregate lines such as “FIELD CROP TOTALS, INCL POTATOES & OTHER” and “CROP TOTALS, (EXCL HORTICULTURE).”

## Data source

The page loads `download.csv` from this folder when it opens. That file is the saved USDA NASS export. On load it had 387 raw rows and 289 usable crop-year values. With a 5-year average, the top suggestions were soybeans, sugarbeets, and hay and haylage. Corn still appears in the ranking as a crop the team already sells.
