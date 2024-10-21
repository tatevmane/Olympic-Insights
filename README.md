# Insights into Olympic history

In this independent exploration, I set out to uncover interesting trends/patterns in historical data and identify potential opportunities for a hypothetical client, which I have assumed to be a sports apparel company. The goal is to inform their expansion into new international markets, improving brand visibility and obtaining a wider customer base. Specifically, I am tasked with identifying emerging success in female sports demonstrating promising sponsorship potential.

The open-source Olympics data from Kaggle spans 120 years (1896 to 2016).

### Variables of interest:
Athlete name, sex, height, weight, NOC (National Olympic Committee), Games (formatted as “Year Season”, ex. “1992 Summer”), Year, Season (Summer or Winter), City (host city), Sport, Event (specific event name within sport category), Medal (received or not)

### Necessary libraries: 
pandas, numpy, scipy, plotly, matplotlib.pyplot, seaborn

### Data Cleaning: 
Imputing missing values, dropping unnecessary variables, converting variable types

### Highlights
- Winter Olympics began in 1924, explaining the lack of prior data.
- Summer and winter games occurred in alternating years after 1992.
- Some research revealed that lower participation in 1956, 1976, and 1980 was associated with boycotts.
year_2016_data = athletes[athletes['Year'] == 2016]

Given my client’s interest in female athletes, it is only appropriate to understand their history in the games.

- There was no female participation in the first Olympic games.
- Only 1.89% of all participants were female in 1900 compared with 45.02% in 2016.
- There was a large jump in 1976 (~5%, slope = 1.28). This can be explained by the addition of several female sports in the Olympics.

### Approaches: Medal and Participant Count
Medalists often gain lots of attention in their home countries. It's also important to track female participation by country to identify emerging talent. 

#### Key Insights:
- Bahrain led in female medals in 2012 and 2016. These successes can empower younger generations, leading to increased participation in sports. Bahrain’s athlete count has been on the up and the pattern is projected to continue.
- A closer look at Serbia reveals almost half its female athletes were on the Volleyball team, which won a Silver medal in 2016. There were 12 medals issued to female volleyball players on Serbian Olympic Team. 

Both the Serbian Volleyball and Bahrain Athletics teams can prove valuable targets for a new campaign.

- 15-year-old gold medalist and diver, Qian, is as a potential star.
- The top performing young female Korean athlete in speed skating is Shim Seok-Hui, who won 3 medals in 2014 at the age of 17.

This sort of young talent is what we need!

#### Conclusion:
This analysis offers my client an opportunity to expand into new markets in different regions of the world: Europe, the Middle East, and Asia. They can look into stocking products related to volleyball, athletics, and skating to align with their goals of increasing brand visibility and customer base.

### Future Directions:
- Train models to predict future trends based on historical data (e.g. time series forecasting).
- Obtain up-to-date data to improve accuracy of trends, analysis, and predictions; 5 new sports were introduced in 2024.
- Consider merging external dataset with population or GDP information for economic analysis.
