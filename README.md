### Olympics-EDA

**Note: All analyses and observations presented herein are derived solely from the dataset available, encompassing information up to the 2016 Rio Olympics**

This repository contains an Exploratory Data Analysis (EDA) of the Olympics dataset. The dataset provides comprehensive information about various aspects of the Olympic Games, including athletes, sports, events, and medals awarded across different editions of the Olympics. 

---------


#### Introduction:

The Olympics stands as one of the most revered and significant sporting events globally, held quadrennially. Its inception dates back to 1896, when the inaugural modern Olympics unfolded in Athens, Greece. According to National Geographic, regional Olympic events trace back even further, to 1776 BC.

The iconic rings within the Olympic emblem symbolize the unity of five continents: Europe, Africa, Asia, the Americas, and Oceania. This representation underscores the spirit of international collaboration and competition that defines the Olympic Games.

---------


#### Dataset Description:

The file **athlete_events.csv** contains 271116 rows and 15 columns. Each row corresponds to an individual athlete competing in an individual Olympic event (athlete_events). The columns are:

• ID - Unique number for each athlete <br>
• Name - Athlete's name <br>
• Sex - M or F <br>
• Age - Integer <br>
• Height - In centimeters <br>
• Weight - In kilograms <br>
• Team - Team name <br>
• NOC (National Olympic Committee) - 3-letter code <br>
• Games - Concatenation of Year and Season <br>
• Year <br>
• Season - Summer/Winter  <br>
• City - Host City <br>
• Sport  <br>
• Event <br>
• Medal - Gold, Silver, Bronze (NA means the athlete did not win any medal) <br>

---------


To create the final dataset for analysis, we merged the `athlete_events.csv` DataFrame with the `noc_regions.csv` DataFrame using Pandas' merge method. This merge operation was performed based on the common column "NOC". By merging this column, we combined the athlete information with the corresponding National Olympic Committee (NOC) region data, thereby enriching the dataset with additional regional context.

---------


#### Observations:
• The country with the highest number of participants since the inception of the Olympics is the **United States**,
with 17,847 participants. Following closely behind are **France** with 11,988 participants and **Great Britain** with 11,404 participants.

• The majority of Olympic participants fall within the age range of 20 to 30 years. Nevertheless, there are only a limited number of athletes aged above 50 years old, as well as some who are below 16 years old, participating in the Olympics.

• It is observed that there is a greater quantity of Olympic sports featured in the Summer Olympics as opposed to the Winter Olympics.

• There is a higher number of male participants (72.51%) as compared to female participants (27.49%).

• The total number of female athletes has demonstrated a consistent upward trend from 1980 to the 2016 Olympics, reaching its peak during the 2016 Olympics, where 6223 female athletes participated

• The 6 gold medals won by athletes over the age of 60 were distributed as follows:

  - 1 gold medal in Art Competitions by Isaac Lazarus Israls
  - 1 gold medal in Roque by Charles Jacobus
  - 3 gold medals in Archery by Lida Peyton "Eliza" Pollock (McMillen-), Galen Carter "G. C." Spencer and Robert W. 
    Williams, Jr.
  - 1 gold medal in Shooting by Oscar Gomer Swahn

• In the Rio Olympics - 2016, the United States secured the highest number of gold medals (137), followed by Great Britain (64), and then Russia (50). Ethiopia, Armenia, and Turkey struggled but managed to secure just one gold medal each.
