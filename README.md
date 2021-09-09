#   **Project 2: AMES HOUSING PREDICTION**
## Problem Statement

- The **aim** of this project is to predict property sales prices for each house using data processing.
- To predict the sale price of the property, I used Linear Regression Model. 
[![ct-1546615904-2uxq0e9jr8-snap-image.webp](https://i.postimg.cc/1X0gTJRW/ct-1546615904-2uxq0e9jr8-snap-image.webp)](https://postimg.cc/PvxrvbwZ)

### Brief Summary:
> Realtors determine house values by looking at various features. Some of them are location of the property, condition of the property, year built, square feet area, heating-AC, garage type, total number of bedrooms and bathrooms, and many more. After this, they will look for similar houses in the neighborhood that were sold recently to get a better estimate of the property (from Mateus Realty). 

### **My Approach:**
- Since I was given 80 features, I followed a simple approach to choose 32 highly correlated features to predict Sales Price of a property. I used boxplots (from Python) to correlate all other features with the Sales Price. BoxPlot draws a box plot to show distributions with respect to categories (from Docstring). One example is shown below where I used this inbuilt python function.
[![Screen-Shot-2021-07-15-at-3-19-51-PM.png](https://i.postimg.cc/hGWxcn0j/Screen-Shot-2021-07-15-at-3-19-51-PM.png)](https://postimg.cc/Wd8twQCL)
- Here the x-axis represents the number of half bathrooms in the basement and y-axis represents the SalePrice of a property. The four boxes represent most of the distribution of the respective number of half bathrooms. The dots represents outliers. 
- Since all the four boxes are in the same SalePrice range and there are many outliers, this means the number of half bathrooms in the basement hardly affects the SalePrice of a property, so it is best to drop this feature.
### **Findings:**
- Out of the given 80 features, following **32 features** are highly correlated with the Sales Price of a property : 
       ['MS SubClass', 'MS Zoning', 'Street', 'Land Contour',
       'Neighborhood', 'Condition 1', 'Overall Qual', 'Year Built',
       'Year Remod/Add', 'Mas Vnr Area', 'Exter Qual', 'Exter Cond',
       'Foundation', 'BsmtFin SF 1', 'Total Bsmt SF', 'Heating QC',
       'Central Air', 'Electrical', 'Gr Liv Area', 'Full Bath', 'Half Bath',
       'Kitchen Qual', 'TotRms AbvGrd', 'Functional', 'Fireplaces',
       'Garage Type', 'Garage Finish', 'Garage Cars', 'Garage Area',
       'Paved Drive', 'Sale Type', 'SalePrice']
### Conclusions And Recommendations :
- The feature, **Gr Liv Area** has the largest coefficient. This shows that the Area of the grade (ground) living area appear to add the most value to a home price.
- **Kitchen Qual_Po** has the largest negative coefficient. This tells us poor Kitchen quality hurt the value of a home the most.
- **Main Recommendation:** To correctly predict the SalesPrice of a property you all (real estate agents) should focus on the above mentioned 32 features (in the Findings). In order to increase the saleprice of a house try to improve **Gr Liv Area, overall quality of home, increase car capacity of garage, increase Type 1 finished area and Kitchen Qual_Po quality,** as you all know that with the increase in sale price your profit will increase too. 
- **Note:** In New York State, the standard real estate agent commission is 5- 6% of the property price.

