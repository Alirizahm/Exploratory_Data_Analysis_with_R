# Exploratory Data Analysis with R
Author's : Aliriza Hamonangan Matondang
## Introduction
Hello everyone, i have tried to study Exploratory Data Analysis with R. I did the analysis based on the plot to find the insight of the dataset. We have made 6 Questions to pratice my analysis to find the insight of the dataset
## Data Information
SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict.
- MSSubClass: The building class
- MSZoning: The general zoning classification
- LotFrontage: Linear feet of street connected to property
- LotArea: Lot size in square feet
- Street: Type of road access
- Alley: Type of alley access
- LotShape: General shape of property
- LandContour: Flatness of the property
- Utilities: Type of utilities available
- LotConfig: Lot configuration
- LandSlope: Slope of property
- Neighborhood: Physical locations within Ames city limits
- Condition1: Proximity to main road or railroad
- Condition2: Proximity to main road or railroad (if a second is present)
- BldgType: Type of dwelling
- HouseStyle: Style of dwelling
- OverallQual: Overall material and finish quality
- OverallCond: Overall condition rating
- YearBuilt: Original construction date
- YearRemodAdd: Remodel date
- RoofStyle: Type of roof
- RoofMatl: Roof material
- Exterior1st: Exterior covering on house
- Exterior2nd: Exterior covering on house (if more than one material)
- MasVnrType: Masonry veneer type
- MasVnrArea: Masonry veneer area in square feet
- ExterQual: Exterior material quality
- ExterCond: Present condition of the material on the exterior
- Foundation: Type of foundation
- BsmtQual: Height of the basement
- BsmtCond: General condition of the basement
- BsmtExposure: Walkout or garden level basement walls
- BsmtFinType1: Quality of basement finished area
- BsmtFinSF1: Type 1 finished square feet
- BsmtFinType2: Quality of second finished area (if present)
- BsmtFinSF2: Type 2 finished square feet
- BsmtUnfSF: Unfinished square feet of basement area
- TotalBsmtSF: Total square feet of basement area
- Heating: Type of heating
- HeatingQC: Heating quality and condition
- CentralAir: Central air conditioning
- Electrical: Electrical system
- 1stFlrSF: First Floor square feet
- 2ndFlrSF: Second floor square feet
- LowQualFinSF: Low quality finished square feet (all floors)
- GrLivArea: Above grade (ground) living area square feet
- BsmtFullBath: Basement full bathrooms
- BsmtHalfBath: Basement half bathrooms
- FullBath: Full bathrooms above grade
- HalfBath: Half baths above grade
- Bedroom: Number of bedrooms above basement level
- Kitchen: Number of kitchens
- KitchenQual: Kitchen quality
- TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
- Functional: Home functionality rating
- Fireplaces: Number of fireplaces
- FireplaceQu: Fireplace quality
- GarageType: Garage location
- GarageYrBlt: Year garage was built
- GarageFinish: Interior finish of the garage
- GarageCars: Size of garage in car capacity
- GarageArea: Size of garage in square feet
- GarageQual: Garage quality
- GarageCond: Garage condition
- PavedDrive: Paved driveway
- WoodDeckSF: Wood deck area in square feet
- OpenPorchSF: Open porch area in square feet
- EnclosedPorch: Enclosed porch area in square feet
- 3SsnPorch: Three season porch area in square feet
- ScreenPorch: Screen porch area in square feet
- PoolArea: Pool area in square feet
- PoolQC: Pool quality
- Fence: Fence quality
- MiscFeature: Miscellaneous feature not covered in other categories
- MiscVal: $Value of miscellaneous feature
- MoSold: Month Sold
- YrSold: Year Sold
- SaleType: Type of sale
- SaleCondition: Condition of sale

## The results
1. Start with the target
<img width="430" alt="000007" src="https://user-images.githubusercontent.com/92624520/162129544-c06f7ac9-ae0a-460c-b1e8-ab357192dbef.png">

- Insight_1 : The data spreads between 1.3e+05 to 2.2e+05 and there are outliers ranging from 3.3e+05 to 7.8e+05 from the distribution of the selling price of the house, the average price is not too expensive. Possibly, the target for selling the house is the middle class.
- Insight_2 : The price of the house may have the same type and have large amount of price. But there are some differences in facilities, so there is a price difference among each house. The difference in price between each house is not quite high.
- Insight_3 : The outliers are most likely to be sold at a high price, because the house is made more luxurious or better than the low price house. But, the high price of house doesn't seem like the focus of selling the house.

2. Find the 5 variables with the strongest correlation (positively or negatively) to SalePrice, and whether the results make sense or not?
<img width="430" alt="000005" src="https://user-images.githubusercontent.com/92624520/162131057-57fd14ac-30f4-4c28-a596-45f88a32bfba.png">

- Insight_1 : OverallQual is the feature rate of the entire material and the house, that is completely finished and can be used immediately. In this feature, there is a positive correlation between SalePrice and OverallQuall. It can be seen, the higher the OverallQuall rate, the higher the SalePrice. Why? Because the higher the OverallQuality rate indicates that better the materials are used, the house is completely finished, and can be used immediately without having to make repairs or additional facilities. According to the price of the house, I think this correlation makes sense.
- Insight_2 : TotalBsmtSF is a feature of the total area of the basement. In this feature, there is a positive correlation between SalePrice and TotalBsmtSF. It is because, the wider the basement area, the higher the price of the house, which indicates that the house will also be wider, and has a different type of house. So that, it can increase the selling value, then the area of the basement is also one of the facilities which can increase the selling price of the house. I think this correlation makes sense.
- Insight_3 : GarageCars is a feature of the size of the garage in the size of a car. In this feature, there is a positive correlation between SalePrice and GarageCars. It is because, the larger the line size in the car size, the more cars that can fit into the garage, so the SalePrice can also increase. The number of cars that can be parked in the garage as a facility and it can indicate the house has a high selling value, because most likely the house is made for the upper middle class. The possibility of GarageCars that the more cars that can be parked, the sale price of the house which has garage cars is in the ouliers area of SalePrice. I think this correlation makes sense.
- Insight_4 : X1stFlrSF is a 1st floor area feature. In this feature, there is a positive correlation between SalePrice and GarageCars. It can be seen, the wider the X1stFlrSF, the higher the SalePrice. It is because, the first floor is the main floor in the house and the first floor is the initial foundation of the house. If the 1st floor is bigger, then the 2nd floor will follow the area of the 1st floor, although most likely it will not be bigger than the 1st floor. So, the bigger the first floor, the higher the SalePrice. I think this correlation makes sense.
- Insight_5 : GarageArea is a feature of the garage area. It can be seen that the wider the GarageArea, the higher the SalePrice. This can happen similar to insight_2 that the wider the garage, the more cars which can be parked and signifies that the wider the garage. With other words, the house is made for the upper middle class and the possibility that SalePrice is in Outliers. However, the wider the garage can also be used for other places such as places for doing automotive activities and etc. It means, the line area also has multiple functions and as a good facility, so that it can increase SalePrice. I think this correlation makes sense.

Note : All of the analyzes given previously must be explored deeper and further, because there are other variables that also have a positive or negative correlation with SalePrice, even if the value is small or large. We must also study deeply and more realistically. It is related to each other correlation among variables.

3. It is never hurt to test basic knowledge
<img width="430" alt="000005" src="https://user-images.githubusercontent.com/92624520/162131683-b7dd3469-09c8-4ad3-8cd2-389b71a2863b.png">

- Insight_1 : We have checked the relationship between OverallQual and SalePrice. It can be seen the higher the OverallQual, the higher the SalePrice.
- Insight_2 : However, this increase is not solely due to an increase in the rate, because for each rate, there is a price increase. For the example, the rate 5 of houses price also tend to increase continuously, so that the increase in house prices is only found at the highest level of price at each rate. So it can be assumed that the increase is not quite significant or massive.
- Insight_3 : The price increase at each rate may occur due to the age of the house or new house, increasing the age of the house results in the house prices increasing because house prices usually increase every year, or there are renovations carried out so that there is an increase in prices at each of these rates.

Note : All of the analyzes given previously must be explored deeply. We have to study deeply and more realistically related to the correlation among each other variables that caused the price increase.

4. Beware of false correlation
<img width="430" alt="000003" src="https://user-images.githubusercontent.com/92624520/162131912-8cac4b4f-d12a-4303-b1a1-7fb235073162.png">

- Insight_1 : Based on the visualization above, SalePrice, OverallQual, and SaleCondition, it can be seen that new houses have a high SalePrice, but not all new houses have a high SalePrice.
- Insight_2 : The SalePrice trend of the new house does not tend to be quite expensive, but there is an increase in SalePrice based on SaleCondition and OverallQual.
- Insight_3 : Partial SaleCondition is a house that has not been completed at the last time the assessment, but is related to a new house. So there is a trend of price increases based on the last assessment, for OverallQual quality that is getting better then SalePrice also increases, as well as normal SaleCondition. So, it can be assumed that there is a positive correlation or relationship between YearBuilt and SalePrice, but it is also influenced by OverallQual and SaleCondition, then SalePrice tends to increase based on OverallQual and SaleCondition, therefore it cannot really be interpreted that new house tend to have SalePrice high because the house is new, there are still several variables that can determine this.

5. Haunted place(?)

<img width="430" alt="000003" src="https://user-images.githubusercontent.com/92624520/162132138-f9629148-de60-4cd1-a8fc-c2c62ae21096.png"> <img width="430" alt="000005" src="https://user-images.githubusercontent.com/92624520/162132194-285ea5bb-736a-4ec5-a2cb-3a07b08997bf.png">

- Insight_1 : Based on the visualization above the Relationship between GrLivArea and SalePrice plot, there is no relationship between Street on SalePrice for the two houses that have a very wide GreenLivingArea on the right of Relationship between GrLivArea and SalePrice plot. Because for the two houses that have a very wide GreenLivingArea they are on the same street, namely Pave
- Insight_2 : Based on checking the "Relationship between GrLivArea, SalePrice, YearBuilt, Street and LandContour plot, the pave street also has various types of LandContour where LandContour "Bnk" has a lower price compared to other LandContours. For the two houses that have GreenLivingArea located on Pave road at LandContour "Bnk". "Bnk" is a sloping or steep land contour where the contour of the land rises high or steeply from the road to the house building, because such a LandContour causes house prices to tend to be cheap even though if you look at the years of building, the houses are new building.
- Insight_3 : LandContour "Bnk" is not quite liked by buyers. The LandContour "Bnk" can also endanger buyers (prone to natural disasters such as landslides, earthquakes, etc.), and also make the buyer uncomfortable. So the price of houses with these contours tends to be cheap even though they have a large GrLivArea

6. Freestyle
<img width="430" alt="000003" src="https://user-images.githubusercontent.com/92624520/162132636-c67e4fa6-16a2-4cba-b5a0-2192f6fb6e73.png">

- Insight_1 : There is an interesting for me from the correlation between OverallCond, OverallQual, and SalePrice, where there is a negative correlation and close to 0. OverallCond is a feature that describes the rating of house condition. If OverallQual is positively correlated with SalePrice, if there is an increase in OverallQual, then SalePrice will also increase. However, this is actually inversely proportional to OverallCond, where OverallCond tends to increase, SalePrice tends to decrease or gather at a certain value so that it is close to 0. OverallCond, OverallQual, and SalePrice should have be possitive correlation each others where if OverallCond (a feature that describes the rating of house condition), OverallQual (all materials and the house is completely finished and can be used immediately) goes up, so the SalePrice (sales price) also goes up. Was there an error while fetching OverallCond data so that the data was not aligned? or we need to do data cleaning or data pre-processing?
- Insight_2 : Based on checking, it can also occur when the OverallCond rating is high but the OverallQual and SalePrice is low because at the time of the assessment the condition of the house is good and decent,but the materials are used by building the house tend not to be quite good, so the reparation of house tends to be faster and costs a lot of money.
- Insight_3 : Based on checking, it could also happen the other way around where the condition of the house is not in good condition, but the material used is good, it only needs to make some repairs and does not cost a lot of repairs, so it can gather at one point that is not far apart, which can cause the data to approach 0.
