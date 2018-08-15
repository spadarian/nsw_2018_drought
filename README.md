# NSW 2018 Drought visualisation
================================

This is a simple visualisation of the drought affecting NSW, Australia in the winter of 2018.

## Methodology

I used the **normalized difference vegetation index** (NDVI) as an indicator of photosynthetic activity. Healthy, growing vegetation show high NDVI values. If vegetation is under any stress (nutrition deficiency, water shortage, etc.) that would affect the photosynthetic activity and result in lower NDVI values detected from satellite imagery.

I estimated the mean NDVI from the Landsat 8 images captured **between June, 1st and August, 15th**. To remove clouds and other artefacts, I only selected the **'clear' pixels** (pixel quality band). Since different crops show different NDVI values, crop rotation can generate misleading results. The same might happen if a farmer decided to leave the land fallow, which would lead to lower NDVI values. To minimise that effect, I used the **mean NDVI value from 2014 to 2017** as the 'past NDVI'.

The final difference was calculated as:

NDVI_diff = (NDVI_2018 - NDVI_past) / NDVI_past

:warning: Note: This is a quick method to visualise the changes in vegetation. **These changes can occur due to many factors and not only drought**. The only thing we know for sure is that **climate change** is modifying rainfall behaviour, so we need to **reduce carbon emissions**, **support renewable energy project**, etc.

:warning: Don't use this map without warning people about its limitations. That is sensationalism.

## Disclaimer

This is a demo for illustrative purposes only and it is provided as-is. Use at your own risk.
