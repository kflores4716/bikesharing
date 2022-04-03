# Bikesharing

## Overview
This analysis was created as part of a business proposal to start a bikesharing business in Des Moines, Iowa. We have attracted some potential investors, however, we would like to prove to them that this will be a successful business so that these backers are confident in their decision to support us. Thus, the goal of this analysis is to tell a statistical story that will prove to our investors that this business will succeed.

#### Applications Used
To complete our bikesharing analysis, we pulled a `.csv` file from the Citi Bike website that contains New York City bikesharing data from August 2019. We then pulled that `.csv` file into Jupyter Notebook and added an extra column. The existing `Tripduration` column was an `integer` datatype, so in the newly added column, we copied that `Tripduration` data and changed the datatype to `datetime`. Once we had this new column, labeled `Tripduration Dt`, we then used Tableau Public to create some visualizations of the updated bikesharing data. In Tableau, we created several `Worksheets` and `Dashboards`, and then added them to a `Story` that will be used to present our analysis to the investors.

## Results
The completed Tableau Story includes data regarding what times and days of the week the bikes are most used. It also includes some gender and age-specific data to show how bike usage differs between these different groups of people. The last few story points include data regarding when bikes are checked out, as well as where they're checked out from and where they're returned to. Please feel free to click the link below and view the Tableau story on the Tableau Public website. Also, please continue reading for more in-depth descriptions of the visualizations included in the story.

![Link to Dashboard](https://public.tableau.com/app/profile/kevin.flores5254/viz/BikesharingAnalysisChallenge/BikesharingStory?publish=yes)


#### Trips by Weekday & Customer Type

![Trips by Weekday per Hour](https://user-images.githubusercontent.com/94764735/161439101-bce31cb9-afbd-4fad-b910-1f7304424a43.png)

This first visualization in the story gives us an idea as to what time of day the bikes are checked out most often. The chart plots the stoptime in hours along with the all the days of the week, and it shows us that the bikes are most often used in the mornings and in the evenings. This can mean a few different things:

- The high usage in the morning could mean that a good number of people might use the bikes to get to work. 
- The high usage in the evening would then mean that those people who used the bikes to get to work in the morning are also using them to get back home.
- Regarding tourists who use the bikes, it would make sense for them to follow the same pattern. Perhaps they are using the bikes in the morning to get to the attractions they would like to visit, and then are using them in the evening to return to their hotels and maybe even stop for dinner and a show on their way.

The second visualization in this story point is a pie chart showing the split between short term customers and annual subscribers of the service. We can tell from the pie chart that over 75% of the users are annual subscribers, while the rest of them are just occasional customers. Although there could be some tourists who are subscribers to the service, it is likely that the majority of annual subscribers live in NYC. Thus, this leads to the conclusion that the majority of citi bike users in this dataset are NYC locals and not tourists. This conclusion regarding customers and subscribers is important to keep in mind throughout the entire Tableau analysis, which is why we included it in the very first story point.

#### Gender Usage Data

![Gender Usage Data](https://user-images.githubusercontent.com/94764735/161439115-4579bd6d-b8e4-485b-a573-8047c279dcbc.png)

The first visualization in this next story point gives us a breakdown of User Trips based on gender. It also filters the data according to the day of the week, and splits it up between short term customers and annual subscribers. Perhaps the most obvious pattern here is that it shows us (again) that the bikes are mostly used by subscribers as opposed to short term customers. Another pattern we can see is that there are far more male subscribers than female subscribers. It's hard to figure why men use citi bikes far more than women, but it does tell us that there may be an opportunity to increase usage perhaps by marketing directly towards females to try and increase their bike usage.

The second vizualization splits up our previous `Trips by Weekday per Hour` visualization by gender to see if there are any differences. This split visualization shows us that there really isn't a difference between male, female, and unknown genders regarding what time of the day they use the bikes. Here we can conclude that all genders probably use the bikes for the same reasons, such as getting to and from work, or getting to certain attractions or events. 

#### Average Trip Duration by Age

![Average Trip Duration by Age](https://user-images.githubusercontent.com/94764735/161439124-49dbe7c3-cae8-497a-8abc-3cd68a153349.png)

This next story point contains a single visualization showing the average trip duration according to the rider's age. Looking at the second half of the graph, there is a subtle yet obvious trend showing us that average trip duration increases as the rider's age decreases. This result is no surprise as the older people get, the less they are able to do things such as bike to and from places. It's a bit curious, however, why there is data listed for riders who were supposedly born in the late 1800's and early 1900's, as they would definitely not be fit to ride a bike around town these days. Perhaps this can be accounted to rider's making a mistake when entering their date of birth? Whatever the reason may be, it likely can be accounted to some sort of error since the first half of the graph seems to be randomly distributed, not really following a pattern of any sort. So, disregarding that first half, the data here is showing us a positive correlation between birth year and average trip duration, meaning that there is a negative correlation between average trip duration and age.

#### Checkout Times for Users and by Gender

![Checkout Times for Users and by Gender](https://user-images.githubusercontent.com/94764735/161439127-ca2a6c55-081f-4b34-bc69-59abed99e5bd.png)

Moving on to the next story point, we include two graphs visualizing how long the riders checkout the bikes for. The top graph includes data for all genders, and it tells us that the vast majority of riders use a citi bike for less than one hour. In fact, most riders actually only use a bike for less than half an hour, with the peak ride duration falling around 5 minutes per ride. The bottom graph splits this data to see if these ride durations vary by gender, but judging by the graphs this is not the case. 

These visualizations shed some more light on the reasons why riders checkout bikes in the first place. Obviously, the riders are using the bikes to (more quickly) get from one place to another, but since the majority of ride durations are less than 30 minutes we can deduce that wherever the riders are going, it probably isn't too far away.

#### Top Starting and Ending Locations

![Top Starting and Ending Locations](https://user-images.githubusercontent.com/94764735/161439135-f648606e-df7a-4c58-ac2e-bb4b4bd2edef.png)

The final story point included contains two maps, one showing the top starting locations and the other showing the top ending locations. Mapping this data is an essential part of the analysis because it will inform us on which areas of the city we should increase or decrease our bike placement. Comparing the two maps side-by-side, we can see that they are nearly identical. This hints at the possibility that riders are most likely to end their trip at the same place they started. Or it at least shows us where the most popular bike stations are. 


## Summary

### Overall Analysis of the Bikesharing Data

After reviewing the entire analysis, there are a few main points that can be deduced:

- The bikes get the most use during the mornings and evenings.
- There are far more male riders than female riders, and of all these riders, the majority have annual subscriptions.
- The younger the rider, the longer their trip duration.
- The majority of trips are less then 30 minutes long.
- The top starting locations are also the top ending locations.

Using this data and these deductions, we can begin to develope a strategy for our new bikesharing business in Des Moines. We know when the bikes tend to be used the most, so we know that the nights/early mornings are the best times to clean and maintain them so that they remain in working order. We also know that the bikes are mainly used by men. Perhaps when first starting out, we can gear our advertising more towards women to try and close that gender usage gap. 

Regarding the split between short term users and annual subscribers, we might want to keep this in mind and revisit it after we have been in operation for a bit. In a city such as New York, it is almost a nuisance to own/rent a car and drive to and from your destination. Thus, they have numerous methods of public transportation. However, a city like Des Moines is more spread out making it easier for people to drive places. Perhaps NYC has so many subscribers because they have plenty of vehicle-less residents and tourists who need a way to get where they're going. Whatever the reason may be, it would be wise to prepare to have a different distribution of short term users and subscribers. Once we are up and running, we could then perhaps start targeting our ad campaigns to increase the count of whichever type of rider might be lacking. Additionally, we should be more weary of our earlier assumption that riders are using the bikes to get to and from work. If people in Des Moines really are more likely to drive places, then one of the many places they would drive would certainly be to and from work. 

The outcome of our age-specific data is something that could have been assumed before the analysis. However, it is always good to have analytical evidence that the younger riders tend to ride for a longer duration. Regarding ride duration as a whole, our analysis outcomes tell us that riders are not riding the same bike for the entire day. With most ride durations being less then 30 minutes, we can also deduce that riders probably aren't biking too far. While this makes sense in such a dense city as NYC, we might want to be prepared for some different trends in Des Moines. Since things aren't as crowded in Des Moines, it may take people longer to get where they're going, which then would increase ride durations as a whole. This should especially be kept in consideration because if someone's destination is sufficiently far away, they will be more inclined to seek other, less tiring methods of transportation.

Lastly, we have the starting and ending location data. These outcomes will likely not be as affected by the differences in city layout between NYC and Des Moines. It makes complete sense that the most popular starting and ending locations are virtually the same. We have deduced that riders are almost always using the bikes to get from one place to another (not for exercise), thus, the place that they are going must be a place worth going to. Wether it be restaurants, stores, events, you name it, the riders have a reason to go there. If there is a reason to go, they won't be the only ones, so the more popular the destination, the more traffic the nearby bike stations will get. It also follows that these popular destinations will likely have people there already who will need to grab a bike to get back home. Thus, bikes are probably exchanged pretty frequently through these popular stations, meaning that these  places will serve as almost equally high ending destinations as starting destinations. This conclusion offers some peace of mind, as we will not have to worry as much about not having enough bikes (or having too many bikes trying to be returned) at certain stations.

Although these visualizations offer useful insight, perhaps including additional data would help develope a more concrete plan for rolling out our Des Moines bikesharing business. One such visualization that would be very useful is if we had a chart showing us how users are split between residents and tourists. If we knew it was mostly tourists, we could focus on positioning stations near tourist attractions. If there were substantial residents, we could make sure to position stations in popular residential areas. Although we already made an assumption from the NYC data that most users are residents, it would be much more comforting if we actually had concrete evidence. Furthermore, another visualization that would help us would be a graph showing `Usertype` (subscriber vs short term) and `Tripduration`. We already have a story point showing popular usage times and days of the week based on usertype, but knowing how long each type of user tends to ride for would tell us even more. Knowing this would help us draw conclusions as to why short term users are riding our bikes, and might help us figure out how to turn these temporary users into annual subscribers. Lastly, if we added more layers to our top starting and ending locations maps, we would get a much better idea of why certain stations are so popular. For example, adding `Tripduration` to these maps would help use figure out how far people are biking to get to their destination. If users are biking for an especially long time, that would tell us that their ending station is close to something that is worth visiting. We could even go further by searching for a map of the most popular locations in the city and layering it on to our existing maps, thus properly visualizing the link between most popular starting/ending locations and theses popular city sites. 

While additional visualizations would certainly help with our analysis, what we have so far is a good start and has already given us some great ideas for our new business venture!

