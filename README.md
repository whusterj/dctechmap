dctechmap
=========
The DC Tech Map is a map of startups, coworking spaces, digital agencies and corporate technology offices throughout the DC area. 

We currently feature the following firms:
* 18F
* 3Advance
* APCO Worldwide
* Contactually 
* Deloitte Digital
* OPOWER
* Rock Creek Strategic Marketing
* Routeam 
* Sunlight Labs
* TrackMaven

### Want to add yourself to the list?

1. Look up your address in Google Maps. In the URL, you'll notice two numbers preceded by an @ symbol that likely start with a 38 and a -77. Those are your coordinates you'll need for the geojson file.
2. Update the offices.geojson file. Your entry will look something like the following:
```json
{
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -77.028078,
      38.898315
    ]
  },
  "properties": {
    "marker-symbol": "commercial",
    "name": "APCO Worldwide",
    "address": "700 12th St NW"
  }
}
```

The `marker-symbol` tag comes from [Mapbox's Maki library](https://www.mapbox.com/maki/). Hover over the icon you want to get the tag name. Make sure to validate that your GeoJSON works using the [GeoJSON linter](http://geojsonlint.com/).

Submit a pull request and I'll plug you in.
