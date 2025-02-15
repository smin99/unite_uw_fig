# Broadband Provider Investigation

Ryker Bukowski, Seungmin Hwang, Kevin Wang, Howard Xiao

[View a demo on ShinyApps.io.](https://ktw0222.shinyapps.io/fishery_wifi/) Please give the data time to download.

# Advertised Internet Speeds Across the United States

This data set is available online, provided by the Federal Communications Commission (FCC). All Internet Service Providers (ISP) are required to submit their advertised internet rates every six months. The information was last updated March 20, 2018. This data is made available to the public through the FCC on their website, located [here]( https://opendata.fcc.gov/Wireline/Fixed-Broadband-Deployment-Data-December-2016-Stat/b5f4-szwq).

Something of note: This information is the claimed or advertised rates of internet service, which may differ from the actual rates which consumers will receive.


### About the Data

<img src="fcc.png" height="100px">

The [data set](https://opendata.fcc.gov/Wireline/Fixed-Broadband-Deployment-Data-June-2017-Status-V/9r8r-g7ut) provided by the FCC is very large, roughly 4 gigabytes. Within the data, there are 68.4 million rows of information, spanning across 17 columns. Due to the size of the data and the amount of information within, the group created a smaller random sample (using `shuf`) to use in the project, due to the idea that if a data is correctly randomly sampled the statistics would still be representative of the entire data set. After this was done, the information used was only a fraction of the size, allowing the teams computers to more efficiently sort through the data set. 

### How the Data is Desplayed

The project decided to display the information provided by the FCC in several different ways. The first set of information shown is a heat map of the contiguous United States, separated by state and the averages of advertised internet speeds. Under this set of data is text which displays information relating to the heat map. The next table is used to display rates of upload and download speeds. Following the map, text and table, a pie chart displays each selected state information. Breaking down the information even further into a distribution of internet speeds available, as well as the proportion of consumers who have specific internet plans. 

### Importance 

This data is important for consumers to have, because it gives them the information in which they need to fully understand what is available to them. Data rates and speeds change based on location and state and is an important factor to take into consideration when making a variety of decisions and this data and visualization can be an important resource. 

# Usage

## Data gathering

The data that was prepared for this presentation is available in the `data/` directory. The script that creates this dataset, with full instructions in the comments, is provided in `scripts/make_data.R`, which you may also elect to follow from the comfort of your own home.

## Presentation

This project is presented using an RShiny app. The actual app is located in the project directory, which can be run locally or uploaded to a third party hosting service like ShinyApps.io.

## Dependencies

If you do choose to run it locally, install dependencies necessary by:

`install.packages(c("shiny", "shinydashboard", "data.table", "mapdata", "ggplot2", "dplyr", "kableExtra"))`

