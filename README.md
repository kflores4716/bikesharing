# Bikesharing

## Overview
This analysis was created as part of a business proposal to start a bikesharing business in Des Moines, Iowa. We have attracted some potential investors, however, we would like to prove to them that this will be a successful business so that these backers are confident in their decision to support us. Thus, the goal of this analysis is to tell a statistical story that will prove to our investors that this business will succeed.

#### Applications Used
To complete our bikesharing analysis, we pulled a `.csv` file from the Citi Bike website that contains New York City bikesharing data from August 2019. We then pulled that `.csv` file into Jupyter Notebook and added an extra column. The existing `Tripduration` column was an `integer` datatype, so in the newly added column, we copied that `Tripduration` data and changed the datatype to `datetime`. Once we had this new column, labeled `Tripduration Dt`, we then used Tableau Public to create some visualizations of the updated bikesharing data. Ine Tableau, we created several `Worksheets` and `Dashboards`, and then added them to a `Story` that will be used to present our analysis to the investors.

## Results
The completed Tableau Story includes data regarding what times and days of the week the bikes are most used. It also includes some gender and age-specific data to show how bike usage differs between these different groups of people. The last few story points include data regarding when bikes are checked out, as well as where they're checked out at and where they're returned to. Please feel free to click the link below and view the Tableau story on the Tableau Public website. Also, please continue reading for more in-depth descriptions of the visualizations included in the story.


##### Trips by Weekday & Customer Type

ADD IMAGE OF THE PAGE HERE!!!

This first visualization in the story gives us an idea as to what time of day the bikes are checked out most often. The chart plots the Stoptime in hours along with the all the days of the week. The chart shows us that the bikes are most often used in the mornings and in the evenings. This can mean a few different things:

- The high usage in the morning could mean that a good number of people might use the bikes to get to work. 
- The high usage in the evening would then mean that those people who used the bikes to get to work in the morning are also using them to get back home.
- Regarding tourists who use the bikes, it would make sense for them to follow the same pattern. Perhaps they are using the bikes in the morning to get to the attractions they would like to visit, and then are using them in the evening to return to their hotels and maybe even stop for dinner on their way.

The second visualization in this story point is a pie chart showing the split between short term customers and annual subscribers of the service. We can tell from the pie chart that over 75% of the users are annual subscribers, while the rest of them are just occasional customers. Although there could be some tourists who are subscribers to the service, it is likely that the majority of annual subscribers live in NYC. Thus, we can conclude that the majority of citi bike users are NYC locals and not tourists. This conclusion is important to keep in mind throughout the entire Tableau analysis, which is why we included it in the very first story point.

##### Gender Usage Data

ADD THE PAGE HERE!!!

The first visualization in this next story point gives us a breakdown of User Trips based on gender. It also filters the data according to the day of the week, and splits it up between short term customers and annual subscribers. Perhaps the most obvious pattern we can see is that there are far more male subscribers than female subscribers. It's hard to figure why men use citi bikes far more than women, but it does tell us that there may be an opportunity to increase usage perhaps by launching a marketing campaign focused on increasing female bike usage.
