---
title: Life Choices REST API References

language_tabs:

toc_footers:
  - <a href='https://github.com/cmpe273-indexzero/life-choices-WS'>View WS Project GitHub Page</a>
  - <a href='https://github.com/cmpe273-indexzero/life-choices-iOS'>View iOS Project GitHub Page</a>

includes:
  - errors

---

# Introduction

Welcome to the Life Choices API!






# GEO Web Services
## POST Geo History

path: `POST /v1/geo/`

consumes `application/json`

produces `application/json`


> {
>    "userName":"maksim",
>    "timestamp":1394932551,
>    "latitude" : 37.415365 ,
>    "longitude" : -122.089803
> }


Response type: **application/json**
Response Payload Sample:

> {
>     "id":"5324fb6803647201bbbfe4da",
>     "timestamp":1.39493261E9,
>     "latitude":37.415363,
>     "longitude":-122.089806,
>     "userName":"maksim"
> }

Response Status: **201 Created**





#Food

##GET Food Places (Yelp API)

####path: `GET /v1/food`

Parameter | Required | Default | Description
--------- | -------  | --------|-----------
latitude  | true     |         | Latitude
longitude | true     |         | Longitude
keyword   | false    |         | Keyword of the search
radius    | false    | 1610 * 3| Search radius
deals     | false    | false   | Show deals only

####produces: `application/json`







#Places
##All Available Places Types

###Request

`GET /v1/places/types`

###Produces

`application/json`

###Response:

> [
> "accounting","airport","amusement_park","aquarium","art_gallery","atm","bakery","bank","bar","beauty_salon","bicycle_store",
> "book_store","bowling_alley","bus_station","cafe","campground","car_dealer","car_rental","car_repair","car_wash","casino","cemetery","church","city_hall","clothing_store","convenience_store","courthouse","dentist",
> "department_store","doctor","electrician","electronics_store","embassy","establishment",
> "finance","fire_station","florist","food","funeral_home","furniture_store",
> "gas_station","general_contractor","grocery_or_supermarket","gym","hair_care","hardware_store","health","hindu_temple","home_goods_store","hospital","insurance_agency","jewelry_store","laundry",
> "lawyer","library","liquor_store","local_government_office","locksmith",
> "lodging","meal_delivery","meal_takeaway","mosque","movie_rental","movie_theater","moving_company","museum","night_club",
> "painter","park","parking","pet_store","pharmacy","physiotherapist","place_of_worship","plumber","police",
> "post_office","real_estate_agency","restaurant","roofing_contractor","rv_park","school","shoe_store","shopping_mall","spa","stadium","storage","store","subway_station","synagogue","taxi_stand","train_station","travel_agency","university","veterinary_care","zoo"
> ]


