# Weatherapp

There was a beautiful idea of building an app that would show the upcoming weather. The developers wrote a nice backend and a frontend following the latest principles and - to be honest - bells and whistles. However, the developers did not remember to add any information about the infrastructure or even setup instructions in the source code.

Luckily we now have [docker compose](https://docs.docker.com/compose/) saving us from installing the tools on our computer, and making sure the app looks (and is) the same in development and in production. All we need is someone to add the few missing files!

## Changes to original app

* App is dockerized and ready to be deployed with docker compose.

* Backend is deployed in Google Cloud Platform. (Endpoint is https://weatherapp-image-6hpb2mtbpa-lz.a.run.app/api/weather)

## Running the app

Add your api key from [openweathermap](http://openweathermap.org/) to docker-compose APPID.

Add the endpoint address to docker-compose ENDPOINT.

And run: `docker-compose up`

## Testing GCP deployment

For example using postman sending a GET request to the enpoint [url](https://weatherapp-image-6hpb2mtbpa-lz.a.run.app/api/weather) returns the weather. :)