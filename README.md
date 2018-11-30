# Photo Location As GeoJSON

This little tool will extract GPS coordinates from your photos and use the locations to create
GeoJSON.

Using the tool is simple. You just give the filenames of your photos as arguments and you will get
GeoJSON on stdout:

```
$ ./plag --pretty photo1.jpg photo2.jpg
{
  "features": [
    {
      "geometry": {
        "coordinates": [
          -121.06083333333333,
          48.47138888888889
        ],
        "type": "Point"
      },
      "properties": {},
      "type": "Feature"
    },
    {
      "geometry": {
        "coordinates": [
          -122.70194444444445,
          45.51888888888889
        ],
        "type": "Point"
      },
      "properties": {},
      "type": "Feature"
    }
  ],
  "type": "FeatureCollection"
}
```
