# CitiBike Analysis Findings & Conclusions

![CitiBike-Logo](CitiBike_Logo_p.svg)

## [CitiBike Analysis Tableau Story](https://public.tableau.com/profile/jen.barny6168#!/vizhome/citibike_15872623997270/CitiBikeApril-October2019)

Data Source: April 2019 - October 2019 datasets from [Citi Bike Data](https://www.citibikenyc.com/system-data).

### Dashboard 1--City Official Map

This dashboard shows a map of all NYC CitiBike stations used between April and October 2019 with zip code labels and boundaries. Marker size and shade indicate the usage of the station--the darker and larger the marker, the more frequently bicicycles are used at that station.  

The map initiates with the aggregate usage over the entire period. City officials may navigate thru each month of the period using the slider located above the top right corner of the map. They will find, unsurprisingly, that CitiBike usage increases as weather improves while the seasons progress from spring thru early summer, reach a peak in late summer, and decline again thru autumn when the temperature drops again. Users also have the option of clicking on the map to isolate a specific station and observing the change in usage over the period. Hovering over each station reveals a tooltip to include the station name and number of rides in the displayed period (either a single month or all months).

This map exposes the most and least utilized CitiBike stations. The vast majority of usage occurs in Manhattan, with limited usage in the outer boroughs. The three most visited stations are Pershing Square North (Grand Central Station), E 17th St & Broadway (Union Square), and 8th Ave & W 31st St (Penn Station)--all of which are major hubs for commuters who live outside of Manhattan. This suggests that many people depend on CitiBike for commuting to and from work. We can investigate this further on the rider analysis dashboard.

### Dashboard 2--Rider Analysis

This dashboard includes two interactive maps (one for origin stations and one for destination stations) and four interactive charts (two for hourly data, two for gender data).

The hourly bar charts are colorized by user type--customers (1-day or 3-day pass users) or subscribers (annual subscribers) and separated into two charts by day--weekdays and weekends. Coloring the bars by user type exposes several trends:

* The vast majority of CitiBike users are annual subscribers.
* The most popular weekday times are during rush hour (7-9am & 5-6pm), suggesting that many subscribers use CitiBikes to commute to and from work (especially utilizing the commuter hub stations mentioned above).
* Most weekend CitiBike users ride in the afternoons, and a much higher number of those users are customers, likely people who are visiting New York or those who use other modes of transportation to commute to and from work.

The two charts at the bottom of this dashboard are colorized by user gender. The pie chart displays gender only, and the horizontal bar chart displays average rider age by gender.  These charts expose several more trends:

* The majority of CitiBike riders are male, about 66% or 2/3 overall.
* The average CitiBike rider is about 38 years old. You will find that although users with unreported gender are typically older than other CitiBike users, they make up less than 10% of all users and their age is weighted less heavily for the average.

When the user begins to interact with the charts, more trends appear. Click on a gender from one of the gender charts to redraw the maps and hourly charts. Female and male riders have similar behavior regarding both stations and hours, but investigating the data for riders with undisclosed genders reveals a few interesting trends: 

* Rides by hour do not follow the same trend as general CitiBike riders--this group is overwhelmingly comprised of customers, not subscribers.
* Unlike CitiBike users as a whole, weekday trip frequency for the undisclosed gender group increase all day until 5pm, then steadily decrease. Weekend trips for this group follow the same trend as the general CitiBike user population.
* The most popular stations for this group are near tourist hotspots--all stations around Central Park, Madison Square Park, Hudson Yards, Brooklyn Bridge Park, Big Apple Greeter (Centre & Chambers Streets), 9/11 Memorial, etc. This, combined with the most common trip times, suggests that most of the CitiBike users who do not disclose their genders are likely tourists. 

### Dashboard 3--Bicycle Analysis

This dashboard includes a dual horizontal bar chart, a line graph and map, each filtered to display only the 50 most frequently used CitiBikes. The bar charts show both the total number of rides and total aggregate ride duration for each of the examined bicycles in the period. It is colorized with a scale from green (least used, and likely in best condition) to red (most used, and likely most in need of maintenance). The line graph provides an additional view of trip frequency to display the most common trip durations (in 5-minute intervals). The map displays where these most frequently used bikes have been. Users may select a Bike ID from the bar charts to recalculate the line graph and map to see the most common trip lengths and most visited stations. This dashboard illustrates the following findings:

* The most used bicycle, by both number of rides and total number of minutes ridden, is ID 35075. Beyond that, there is not a strong correlation between number of trips and total trip duration. Because this set is comprised of the 50 most commonly used CitiBikes, they are all by nature used the most times and have therefore been ridden the most minutes.
* Across all 50 bicycles, the most common single trip duration is 5-10 minutes long. This means users may possibly be taking CitiBikes for shorter journeys and subways or taxis for longer ones.
* Some bicycles are used more commonly in certain areas. For example, bike ID 33758 has been used more commonly up and down Broadway, while bike ID 35067 has been used more widely across the island. Even further, when you click on the 5th Ave & E 88th St station, you will find that one particular bicycle (ID 34412) has been used at that station much more commonly than any other bicycle.
