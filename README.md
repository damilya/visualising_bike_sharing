# Exploring Bike Sharing Data
## by Damilya Zhantayeva


## Dataset

> The dataset consists of information regarding 183,000 records from a bike sharing platform Ford GoBike operating in San Fransisco Bay area. It describes the metrics on each ride such as duration in seconds, start and end time, stations names, member types, gender of the users, their age. The data can be found at this link: https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv. Additional data for other regions is available at this link: https://github.com/BetaNYC/Bike-Share-Data-Best-Practices/wiki/Bike-Share-Data-Systems.


## Summary of Findings

> During exploration, I found out that an average bike ride was around 40 minuts long. But I also found some extreme cases when people rented a bike for 20-23 hours. The most active users are people in their end 20s and early 30s, these users also tend to do the longest rides across all age groups. While some data entries with an age of 100 plus were found. I derived it is the best to cut these extreme outliers from a dataset along with the extremely long rides and saved the changes to a local copy dataframe. After this change, the cutoff age became 80 years old, and cutoff duration of a ride became 50 minutes. The duration of each ride done by people between 60 and 80 years old was significantly shorter compared to people in their 50s and younger, except for people between 18 and 20 years old. While age had a clear effect on the duration of a ride, gender had less impact. One point worth mentioning, the longest rides were conducted mostly by males. Also males strongly prefer to subscribe to a platform compared to females and others. While all three genders overall orefer to use subscription over customer type. However, in the last part I found out that customers tend to take longer rides compared to subscribers. The same holds for all three genders. Interestingly, females on average take longer rides regardless of their user type compared to other two genders. To finalyse our exploration, we checked more insights about the users. Even though, overall Males tend to use Subscription model, Males in their end 20s use the model way less compared to othe age groups of the same category. But Males aged 45 plus are the most consistent users among all genders of that age group. Other gender gave us an interesting observation, that Other Subsribers and Customers have an opposite to each other trend in their 50s and 60s. 


## Key Insights for Presentation

> For the presentation I will focus on KYC for Ford GoBike platform.
> I will first, check the distribution of the age among the members of the platform. The age can be derived from a member birth year provided in the dataset. The latest record in the dataset is of 2019, thus the age is derived based on that year. The distribution will help to see a general trend among the members, find the minimum and maximum ages, an age range of the most and the least active users. 
> Next, I will look into the relationship between the age of a member and the duration of a ride. We might expect a certain behaviour due to a natural bias, but the heatmap will help to assist with making a clear correlation of which age range tends to take the shortest or longest rides as well as to see which age range takes the greatest number of rides and on which distance.
> Finally, I will conclude with the violin plots on members' gender and user types to members' age. I will showcase how a spesific membership type and gender correlate with the age.