# Machine Learning Crime Rate Analysis

# Why?
The security and stability of our homes can have dramatic influences on our lives. It should therefore come as no surprise that violent crime is correlated with neighbourhood characteristics, such as segregation and social capital, according to Sackett (2016).

This led us to wonder whether it is possible to predict the level of crime in a town based on neighbourhood characteristics. From this, we developed our research question: are social factors (ie: lower status populations (LSTAT)), infrastructure (ie: accessibility to radial highways (RAD), and the number of non-retail businesses (INDUS), or government policies (ie: property tax rates (TAX)) most effective at predicting per capita crime rates in Boston? We chose a variety of neighbourhood characteristics to investigate if social factors, infrastructure, or legislative decisions are the most impactful on crime rates.

In order to test our research question, we will be using real-estate data collected from suburban towns in Boston.
We do NOT own the data within data.csv 
To replicate our findings, the csv data file can be downloaded from Kaggle at: https://www.kaggle.com/arslanali4343/real-estate-dataset.

# Methods
We have determined that we will encounter a standard amount of cleaning and data wrangling.

The variables with which we are going to use to predict the level of crime in the town is LSTAT, RAD, INDUS and TAX determined by the value of correlation to CRIM within the summary function. This project will help us visualise whether these socioeconomic and political factors has any effect on the capita crime rate by town (CRIM). In particular, we are using a real estate data set surveyed over the Boston suburban area by Dragon Real Estate.

After tidying up the original dataset, separate K-nearest neighbours (K-NN) regression analyses will be used to determine the relationship between the mentioned predictor variables and CRIM. To ensure a best-fit regression plot, a tuning model for the number of neighbours will be utilised to determine the best K value. Furthermore, the variables will be standardised if needed to account for differences in the range/units of variables. The resulting regression plots will be visualised in scatterplot form.

Steps:
1. Read Data from a Github Repo where we put our data.csv file that was downloaded from Kaggle
2. Seperating Training and Testing data, eliminating and testing NAs
3. Data Summarization using both "summary" and our self-defined function
4. Data visualization
   -  We first use ggpairs() function to see and decide which features have the strongest 
      correlation with the prediciton CRIM, among which we chose the ones that would make 
      sense in real life.
5. Graph the most suited predictors against CRIM and observe how the data points distribuite


# Expected outcomes and significance
Historically, poorer neighbourhoods have higher rates of violent crime according to Quillian and Pager (2001). Therefore, we expect social factors (ie: LSTAT) will be able to most accurately predict the per capita crime rate of a town.

Information about the importance of social, infrastructural, and policy factors will be useful to policymakers. It will help identify where they should focus community resources and which programs they should endorse. Whichever factor is identified as the most influential will encourage us to question if other neighbourhood characteristics from the same factor are also equally as useful at predicting per capita crime rates.

Me and my teammates own all the code in this Repo. 
