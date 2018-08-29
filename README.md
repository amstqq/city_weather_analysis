# Weather Analysis

This is a two-part project aiming to visualize global weather trend. The first part of the project uses OpenWeatherMap API, Python requests, and JSON traversals to obtain weather data about 500+ random cities across the globe and create a representative model of weather across world cities. The second part of the project is a visualization dashboard website built with models and analysis obtained from part I. The website will contain all visualizations along with their corresponding explanations as well as the data used to create these visualizations.  

Your objective is to build a series of scatter plots to showcase the following relationships:


Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

## Navigation
- data_analysis folder contains all jupyter notebooks used to process data and create visulizations.
- data_gathering_cleaning folder contains jupyter notebooks used to clean the data and perform API calls to collect information about popular Youtube videos
- photos folder contains all visualizations.
- trending_data_csv contains cleaned version of kaggle dataset.

## Data Cleaning and Processing
- Videos with NAN video_id and title are filtered out
- category_id, views, likes, dislikes, comment_count columns have their data type changed from object to numeric

### Dealing with Duplicates

A list of trending videos from Youtube are appended to the dataset daily. As a result, if a video stays trending for more than one day, it will be appended to the dataset multiple times.

When calculating the number of days it takes for a video to beocome trending after it is published, if a video has duplicates, only the video with the earliest trending_date is kept as this date indicates the first time the video becomes trending. All other duplicates are removed. Then, the difference in days  between trending_date and publish_date is calculated

When calculating the number of days a video stays trending, duplicates are kept as the simply the number of duplicates indicates the number of trending days.

## Findings ##

**Does video category impact the number of trending videos and average views?**

    1. There is significant variation in the number of trending videos per category. The Entertainment category had over 25% of all the trending videos in our sample. S number of categories had no videos, and some categories such as Shows and Nonprofits/Activism had very few trending videos videos.

    2. Out of categories with a larger sample, Music videos had the most average views per video, followed by Gaming.

    3. Music and Gaming also had the highest number of comments per video on average which suggests that these categories drive higher engagement.

**Does video category impact how long a video takes to trend and how long it trends for?**

    1. Shows and Nonprofits/Activism had the shortest average time to trending, but they had very small samples. Travel & Events, Howto & Style, and Pets & Animals had the fastest time to trending among larger sample size categories. On the other hand, Autos and Film & Animation took the longest amount of days to trend on average.

    2. Music and Gaming stayed trending for the longest number of days, whereas Sports and News/Politics trended for the shortest number of days.

**Is there variation in how many views each category receives per month?**

    1. There is variation in how many views some categories received by month. Some categories, such as Education and Pets were relatively stable, whereas others such as People/Blogs and Film/Animation had wide variations in views over the 6 months. The sample for some of these categories was fairly low so the data needs a larger sample. Certain categories may be impacted by events such as The Oscars.

**Does the percentage of likes and dislikes vary by category?**

    1. Comedy and Education had the highest percentage of likes whereas News/Politics and Autos/Vehicles had the lowest percentage of likes.

    2. Gaming had the highest percentage of dislikes, while Autos/Vehicles had the lowest percentage of dislikes.

**Is video description sentiment positive on average? Does it vary by category?**

    1. On average, video descriptions have a positive sentiment.

    2. There were categories that showed a lower average sentiment, including News/Politics and Music. Education and Howto/Style showed the highest average description sentiment.
