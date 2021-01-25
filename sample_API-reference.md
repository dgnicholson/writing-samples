# COVID-19 API
Fetches data about COVID-19 from around the world, including the number of cases that are confirmed, critical, and total deaths. This data refreshes every 15 minutes. 


## COVID-19 Numbers by Named Country
`GET` /country/**{country}**

Provides the latest data about COVID-19 for a named country. 


### Request parameters

| Parameter | Required | Description | Type | Default |
|---|---|---|---|---|
| country | TRUE | Name of the country being searched | String | - | 
| format | FALSE | Format of the response (XML or JSON). | String | json | 

### Sample request
```BASH
curl -L -X GET 'https://covid-19-data.p.rapidapi.com/country?name=canada' \
-H 'x-rapidapi-key: {api_key}
```

### Sample response
```JSON
{
    "country": "Canada",
    "code": "CA",
    "confirmed": 659171,
    "recovered": 557652,
    "critical": 843,
    "deaths": 16938,
    "latitude": 56.130366,
    "longitude": -106.346771,
    "lastChange": "2021-01-10T20:44:07+01:00",
    "lastUpdate": "2021-01-10T23:45:04+01:00"
}
``` 
<div style="page-break-after: always;"></div>

## COVID-19 numbers by country code
`GET` /country/code/**{code}**

Provides the latest COVID-19 data for a specified country code. 


### Request parameters

| Parameter | Required | Description | Type | Default |
|---|---|---|---|---|
| code | TRUE | Country code of the country being searched. Must use two or three characters [ISO 3166-1](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes) format. | String | - | 
| format | FALSE | Format of the response (XML or JSON). | String | json | 

### Sample request
```BASH
curl -L -X GET 'https://covid-19-data.p.rapidapi.com/country/code/?code=CA' \
-H 'x-rapidapi-key: {api_key}
```

### Sample response
```JSON
{
    "country": "Canada",
    "code": "CA",
    "confirmed": 659171,
    "recovered": 557652,
    "critical": 843,
    "deaths": 16938,
    "latitude": 56.130366,
    "longitude": -106.346771,
    "lastChange": "2021-01-10T20:44:07+01:00",
    "lastUpdate": "2021-01-10T23:45:04+01:00"
}
``` 
<div style="page-break-after: always;"></div>

## COVID-19 numbers for all countries
`GET` /country/all/

Provides the latest COVID-19 data for each country. 

### Request parameters

| Parameter | Required | Description | Type | Default |
|---|---|---|---|---|
| format | FALSE | Format of the response (XML or JSON). | String | json | 

### Sample request
```BASH
curl -L -X GET 'https://covid-19-data.p.rapidapi.com/country/all/' \
-H 'x-rapidapi-key: {api_key}
```

### Sample response
```JSON
{
        "country": "Afghanistan",
        "code": "AF",
        "confirmed": 53522,
        "recovered": 43948,
        "critical": 93,
        "deaths": 2288,
        "latitude": 33.93911,
        "longitude": 67.709953,
        "lastChange": "2021-01-10T09:37:17+01:00",
        "lastUpdate": "2021-01-10T23:45:04+01:00"
    },
    {
        "country": "Åland Islands",
        "code": "AX",
        "confirmed": 0,
        "recovered": 0,
        "critical": 0,
        "deaths": 0,
        "latitude": 60.1995487,
        "longitude": 20.3711715,
        "lastChange": null,
        "lastUpdate": null
    },
    {
        "country": "Albania",
        "code": "AL",
        "confirmed": 63595,
        "recovered": 37648,
        "critical": 39,
        "deaths": 1241,
        "latitude": 41.153332,
        "longitude": 20.168331,
        "lastChange": "2021-01-10T17:09:58+01:00",
        "lastUpdate": "2021-01-10T23:45:04+01:00"
    },
    {
        "country": "Algeria",
        "code": "DZ",
        "confirmed": 102144,
        "recovered": 69212,
        "critical": 42,
        "deaths": 2807,
        "latitude": 28.033886,
        "longitude": 1.659626,
        "lastChange": "2021-01-10T17:35:19+01:00",
        "lastUpdate": "2021-01-10T23:45:04+01:00"
    },

...

```