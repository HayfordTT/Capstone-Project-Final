
```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
## A Suitable Neighborhood To Open a Hotel and Restaurant In Cape Town, South Africa

Hayford Tetteh
Capstone Project: The Battle of Neighborhoods (Week 1)
IBM Data Science Professional Certificate

## Introduction

South Africa, called by some people the 'Rainbow Nation', a title that captures its diversity and 11 official languages. South Africa is a country where creative expression flourishes and its cultural diversity are embodied in its arts and culture. The country boast of vast tourist and heritage sites including wonderful beaches and cities. Tourism has been one of the high revenue generating industry for the country and so is any company that operate within this industry. Whether you visit the naturally beautiful city of Cape Town and the bottle-green hills of its wine valleys or head out on to any of the beautiful beaches, a holiday in Cape Town will tick all the right boxes.

## 1. Discussion of the business problem.
The Suitable Neighbourhood to Open a Hotel and Restaurant in Cape Town.
Coming down to business problem, Narh Bleponi Tourism Company base in Ghana is expanding their operations to South Africa, Cape Town to be precise. The company want to identify the best Neighbourhood in this wonderful city’s highly populated neighbourhood, a suitable location to open a hotel and restaurant as this city is a famous tourist spot. The company is aware there will be many competitors in terms of hotel and restaurant, But keeping them in mind, they need to locate their hotel in place where more people be attracted to, convenient and comfortable for a stay and enjoy a good meal. South Africa and Cape Town for that matter is an ethnic and cultural diverse city, so a blend of foreign and local flavour of restaurant recipes with Italian, American, typical African, Asian and Indian foods must be available to grab their taste.
The challenge is to find a suitable location in this city to open a new hotel and restaurant to attract all local and foreign people in the centre of all famous venues.


## Expected / Interested Audience
75% locals which comprise of Blacks, Whites and Indiands and 25% foreign peoples of all races visit Cape Town at least once in a year. Some people stay for couple of days or more. Also they find some place for hangout or a good meal. Their main focus might be to stay somewhere near to reach venues. Apart from these set of people, students tourists and working professionals are common audience here. So we may need to fascinate them all.

## 2. A description of the data and how it will be used to solve the problem.

### What data will be used?
We will be completely working on Foursquare data from all the neighbourhood in these city to explore and try to locate our new hotel where more venues like church, temples, beach, museums, memorials other venues excluding hotels and restaurants that are present nearby.

### How will we be solving using this data?
The data set has columns such as Name of venues, Categories of venues, Longitude and Latitude of the venues, Neighbourhood, Id, Likes and Distance from a major central points. We will be looking for midpoint area of venues to locate our new hotel. Before that our major focus will be on all venues present in and around the core place of Cape Town. The data frame has a column postalCode with lots of NaN, thus missing values, but each postalCode represent a neighbourhood and there is a column for neighbourhood so it will be dropped.
I will use the Categories column to classify my data in this case we will focus on "Hotels and Restaurants" which then will give us names of hotels and restaurants with their latitudes and longitudes.
The most important column is the distance column which we will use to perform our exploratory data analysis and it will tell us the distance between all the existing hotels and restaurants to the central location and where it will be suitable to open our venue.
For example, if the distance between hotel number 1 and hotel number 2 is 800 metres and the distance between hotel number 1 and hotel number 2 to the central location is 700 mertres and 850 metres respectively, then our new hotel and restaurant could be half way between hotel number 1 and hotel number 2 and closer to the central location about 600 metres or closer.
Even though Cate Town is atracted to all races, there are cuisines that have higher ratings or likes and these is indicated on the Likes column of the data set and therefore we will use the likes column to choose our menu.
