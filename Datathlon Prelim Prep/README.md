# Part 1: Melbourne Datathlon 2019
This week, I'm going to investigate the kinds of problem that was solved during last year's datathlon to get a good idea of the kind of techniques that will be required to be successful in this project. 

What I didn't know until this week, was that there were actually two different datasets, which separated the competition into two different streams. I will endeavour to briefly explore both fields (hopefully without overwhelming myself) to get a good idea of what kind of project is preferrable for my team this year.

All in all, there are two different streams: 
1. The __Data2App Stream__, which explores satellite images in order to predict the timing and quality of sugarcane production in Prosperone, Queensland
2. The __Analytics Stream__, which looks at Stock Market data in order to create optimal trading strategies and _try_ to make the most money.

It might be interesting to also take a look into projects that were successful too in order to see what was trending successfully last year, and what things that may be important this year.

# Part 2: The Data2App Problem: Sugarcane and Satellites
The main idea of this problem is to analyse Sugarcane farming in Prosperone, Queensland. The main task is to build an interactive app (based on a browser) to provide insight into the production of sugarcane over time primarily using satellite data. This task is to fulfill a number of example use examples for farmers, sugar mills, bankers, fertilser vendors and governments for various cases:
- As a farmer, they could use it for
   - Finding ways to improve crop yield via checking the soil quality and planting/harvesting strategies
   - Comparison between crop growth against other farmers
   - Expected yield at the end of the season
- As a Sugar Mill, they can find better forecasts when sugarcane will likely arrive and by how much
- As a banker, they can look at the amount of money that can be loaned to farmers on the basis of the value of their crop harvested
- For the government, they can:
   - Identify regions and people most affected by extreme weather events
   - Identify new plots of land suitable for sugarcane to support the buifuels industry
- For fertiliser vendors, they can know what farms could be targeted to see products and maximise farmers' benefits

## The Main Dataset
The data is released in three batches, which primarily consist of timestamped statellite images of the regions of interest. In the first batch of data, there are 994 Image Files between the 22/12/2016 to 09/08/2019. Tiles are 512 x 512 in height and width (each with an area of approximately 25 Hectares). Images are captured fortnightly, with one image per capture data, per sensing band. 

In addition, tiles also have a _mask_ which corresponds to sugarcane regions, which you can identify easily whether a pixel is likely to be growing sugarcane vs another crop.

- HAVEN'T EXPLORED IN DETAIL: the second and third batch of data
## Alternative Datasets
It is also possible (and likely encouraged) to also combine findings from other (publicly available) datasets! We have these possible options:

- High Resolution maps of soil quality (including water carrying capacity, pH, Nitrogen, Phosphorus, carbon etc.)
- High Resolution maps of regions which are zoned for sugarcane production
- Weekly local sugarcane production reports (_from Wilmar mills_)
- Weekly sugarcane production reports 2018 (_National dataset_)
- Weekly sugarcane production reports 2019 (_National dataset_)

## Complications of the Dataset
One of the biggest challenges of satellite images is cloud cover and the shadows that are cast onto the images. This will ultimately impact the inference process of the datasets, and will need to be worked around in this research.

# Part 3: The Analytics Problem: Optimal Trading Strategy


# Part y: Past Work


# Part x: Final Thoughts

