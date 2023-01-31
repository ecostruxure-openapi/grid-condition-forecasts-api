# Postman Collection

# About

This collection allows developers to test APIs through [Postman](https://www.postman.com/) application.

# Prerequisites

* Postman desktop or web application
* Valid subscription to Schneider Electric API product

## Usage
 
* [Import collection](#import-collection)
* [Configure variables](#configure-variables)
* [Execute](#execute)


## Import collection

Import `Electricity-Gird-Forecast-API.postman_collection.json` to postman. Refer to [postman documentation to import a collection](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-data-into-postman).

## Configure authorization and variables

Provision is provided at collection level to configure variables and authorization which are used across the requests.

![Postman authorization](/static/images/grid-forecast-authorization.png)

![Postman Variables](/static/images/grid-forecast-variables.png)

| Variables|Comments|
|----------|--------|
|host|API server address, se-exchange-uat-sandbox.apigee.net for UAT sandbox, api.exchange.se.com for production.|

 
## Execute

Follow the steps for end to end flow.

1. [Check supported countries](#check-supported-countries)
2. [Check data providers](#check-data-providers)
3. [Get hourly forecast](#get-hourly-forecast)
4. [Get daily forecast](#get-daily-forecast)

### Check supported countrie

Execute `List supported countries` to check supported countries where forecasting data is available.

![List supported countries](/static/images/list-supported-countries.png)

### Check data providers

Execute `List supported forecast providers` to check which data providers are supported for a given country.

![List supported forecast providers](/static/images/list-supported-forecast-providers.png)

### Get hourly forecast

Execute `Get hourly grid forecast` to retrieve hourly forecasted data for a country and optionally filtered for a data provider.

![Get hourly forecast](/static/images/get-hourly-forecast.png)

### Get daily forecast

Execute `Get daily grid forecast` to retrieve daily forecasted data for a country and optionally filtered for a data provider.

![Get daily forecast](/static/images/get-daily-forecast.png)
