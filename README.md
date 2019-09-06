# Weather app

This app is fully functional, you just **Plug and play**! Before that create 2 free accounts, one on [Dark Sky API](https://darksky.net/dev/register) another on [mapbox](https://account.mapbox.com/auth/signup/).

After creating both accounts, you will have your own secret key and access token, go and paste them in `/src/utils/forecast.js` and `/src/utils/geocode.js` respectively. Note that Dark Sky API is giving us forecast data while mapbox API is for geocoding.

## Application structure

### Backend

The backend is a simple JSON based API that returns forecast data based on the location or address provided. Also, it is serving some dynamic pages and it is written in **NodeJS**.

### Frontend

On the home route, there's a search form where you enter a location and hit submit to get forecast data. Other routes are `/about` and `/help`. I used **handlebars**, templating engine, to generate dynamic views. For styling, I used [Bootstrap](https://getbootstrap.com/docs/4.3/layout/overview/). Lastly, I added a basic script for consuming the forecast API documented above.

## Prerequisites

You must have both [NodeJS](https://nodejs.org/en/) and [npm](https://www.npmjs.com/package/npm) installed on your machine.

### Install dependencies

Go inside the root directory and the following command

```
npm install
```

### To start the app

```
node /src/app.js
```

Visit locahost:3000, you can start playing with the app.
