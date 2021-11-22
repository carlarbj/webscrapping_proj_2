# SpaceX missions analysis

This is the second project made for Ironhack Bootcamp in order to put into practice skills we learned as webscrapping / APIs, cleaning the data gathered, uploading it to SQL and preparing it's visualization in Tableau.
## Status

Complete

## Objectives

To analyse if there is any relation beetween the site where the Falcon9 boosters land the landing failure.

## ## Tools used:
 *Pandas library
 
 *API wrapper space-py
 
 *SQL
 
 *Tableau

## Step-by-step
I found an spacex API with a lot of information regarding lauches that took place up to 2020. 

There was a wrapper that made data gathering a lot easier. 

In the dataset, a lot of the data was in the "rocket" column, such as lauching and landing sites, if the booster was reused or not and if the booster landing was successful. 
As all of this information was in only one columns I had to separate all the info and reate funciond to navigate into each dictionary in order to retrieve the data that was in there. 

With all columns ready I could export it to SQL and to a CSV format in order to make the Tableau visualization.

There are 2 dashboards in Tableau. The first one shows the growth and evolution of successful 
launches. The socond one is an interactive board containing where you can select the mission and see its patch, details, and where it lunched from. 

It's interesting that, due to the success of missions, it's reliability grew significantly and the amount of cango sent grew together along the years.

### Also...
SpaceX is also a company that aims to make rockets cheaper, as many of them are expendable. They developed a way of landing their main booster and reusing them in other missions, reducing a lot the cost of their production. 

<img align="left" src="https://live.staticflickr.com/7653/16892430560_4f9c8c16bf_b.jpg" alt="" width="400" height="300" />

<br/>The boosters can land on the ocean, but it's not the most used one, on land (RTLS - Return to Launch/Land Site) or on a Droneship in the ocean (ASDS - Autonomous Spaceport Drone Ship). 
So I wanted to analyse the success of landings both on land and on the drone. (It's important to remember that in case anything goes wrong in landing, payload won't be affected)

In the dataset there were 3 Falcon Heavy missions, which has 3 boosters for heavy cargo, and the 3 of them land, one on the drone (Which I called the main booster) and the other 2 on land.
The 6 "extra boosters" landings were successful (and they land side by side which is wonderful)
<br/>
<br/>

<br/><img align="right" src="https://i.ytimg.com/vi/TthLhqq4JUs/maxresdefault.jpg" alt="" width="201" height="201" />
<img align="right" src="https://media.wired.com/photos/5a7cb68fa2d3835392e1b469/191:100/w_2400,h_1256,c_limit/spacexrocketreturn.jpg" alt="" width="201" height="201" /> <br/>


## Conclusion
Having in mind that in the dataset there are only official missions, there will be a few failures, but there are many things to be noticed. 

Landing on the Droneship has been a lot more used and with almost no failures in missions, guaranteing the reusability and inexpensiveness of future missions. 
