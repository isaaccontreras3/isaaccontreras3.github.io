---
layout: post
title: MTA Turnstile Analysis
---
![_config.yml]({{ https://pixel.nymag.com/imgs/daily/intelligencer/2016/05/26/26-subway-map-1.nocrop.w536.h2147483647.jpg}}/images/subway_map.png)

## Background:

WomenTechWomenYes (WTWY) hosts annual gala in New York City at the end of May each year in order to connect workers in technology. The goal of the gala is to increase the participation of women in technology and build awareness and outreach. The organization is interested in harnessing the power of data analytics to optimize the effectiveness of street team work, which is crucial to their fundraising efforts. The street team will be placed at the entrances to subway stations to market the event.

## Approach:

By analyzing the MTA subway and demographics data of the city, the optimal strategy for the street team can be solved to increase publicity of the gala. In order to predict the ridership behavior of the current year, the data from May of the previous year will be used.

The following sources are used to generate the data:

* [Metropolitan Transit Authority](http://www.mta.info/)
* [NYC Census Factfinder](http://maps.nyc.gov/census/)
* [Digital NYC](http://www.digital.nyc/)

The following map of New York City shows tech companies in blue dots. By observation, there are two major tech hubs: Silicon Alley and Lower Manhattan. Columbia University is another area which can attract aspiring women workers in technology. These are the three regions of focus where the station ridership data will be generated.

```![_config.yml]({{ site.baseurl}}/images/tech_hub_map.png)```

<img src="/images/tech_hub_map.png" width="500">
## Analysis:

The total counts were calculated by the sum of the entries and exits. The MTA ridership data was provided on a daily basis with audits every 4 hours for each turnstile. Each station consisted of multiple turnstiles, so the data must be analyzed for each individual turnstile before analyzing the station data. After compiling the counts per 4 hours and per day for each turnstile, the total counts can be calculated for each station. Shown below is the total ridership in millions for the top 20 stations.

<img src="/images/station_ridership_barh.png" width="600">

* Analysis of the image above here

The top stations can be refined further based on the demographical information and proximity to tech hubs. The following figure shows the ridership in millions per day of the week for the top 10 refined stations.

* Analysis of image below here

<img src="/images/station_day_heat.png" width="600">

Based on the optimal day for each station, the optimal hours with highest ridership can also be analyzed. Here we show the ridership by 4 hour blocks for each station on their optimal day.

* Analysis of image below here

<img src="/images/station_top_day_hour_heat.png" width="600">

* Generate the top 10 stations based on the demographics and region

[insert plot of the top 10- total day]

* Weekdays look like the best- consolidate weekday results and compare hours

[insert plot of station vs hours]

* Find the optimal time for the highest traffic day of each station

[insert plot of station & optimal day vs hours]

* Remove audits with unrealistic amount of entries, set max entries to 10000 per day
[insert histogram]







Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
