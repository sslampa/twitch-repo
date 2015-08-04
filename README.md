# twitch-repo
## 1. Summary
Hearthstone is an online collectible card game with an active competitive community. There are players across the world that stream this game through the site [Twitch](www.twitch.tv). Those players are referred to as streamers. A select few of these streamers are picked up by sponsored teams for reasons such as a unique personality or being a top player. The purpose of this project is to compare each individual streamer, team, and population and answer the two questions: who is the fastest riser and which streamers best fit each team? 

## 2. Code
Cleaning and scraping code can be found in Code - Data Cleaning and Code - Scrape, respectively. I created my own functions in the create_list library to clean make the code in each section more presentable. 

## 3. Datasets
The dataset for this project comes from web scraping the Twitch site every ten minutes for the month of June. The original dataset and all subsets can be found in the Datasets folder.

#### Variables
There are three main variables that will be seen in each section: current_viewers, followers, and count. 
* __current_viewers__ - In the original dataset, this variable will be the amount of viewers at the moment of data collection. When aggregated, it is the average of all those periods of viewer data collection.
* __followers__ - The same as above, but with the followers. Twitch includes a followers feature where a viewer can 'follow' their favorite streamer and, by following, alerts the viewer of when that streamer is streaming. 
* __count__ - This counts the amount of periods a streamer streams. Each period is every ten minutes (i.e. 10:00, 10:10, 10:20, etc), when the data is scraped from the Twitch website.

## 4. Single
#### Main - Population
This section explores the entire population of the dataset. It provides a comparison between tournament streams (streams specifically used for tournament play) and streams owned by individuals. The section attempts to find a correlation between the number of viewers, number of followers, and number of periods streamed.

#### Single - Riser
The definition of a fast rising streamer is a streamer gaining popularity at a large rate. To find a rising streamer requires looking at the percent change and raw number difference. 

#### Single - Best Fit
Best fits for teams are determined by who would give more coverage to each time. Coverage in this case means how long a member streams (whether it be certain hours or days). There is also a minimum requirement of average viewers, followers, number of periods streaming for each streamer to be considered for each team.

## 5. Teams
The Teams folder contains each individual team with their streamers. Each section shows a general overview and makeup of each team.

#### Main - Team
With the population established, this section looks to compare streamers on teams to the overall population using similar plots. Then each team is compared by the frequency they stream by hours and days. The final part sets the cutoff to be used in finding the best fit streamer for each team.







