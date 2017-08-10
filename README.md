# Geocoder by Geodir


## Services

Generally Available

* [Geocoding](https://www.geodir.co/geocoder/#geocoding)
  * Forward (place names ⇢  longitude, latitude)
  
## Installation

```sh
$ npm install --save geodir-geocoder
```

## Usage

Setup:

```js
var client = new GeodirClient('YOUR_ACCESS_TOKEN');
```

Basic usage of the geocoder:

```js
client.geocodeAddressForward('150131','prolongacion ARENALES 456')
  .then(function(res) {
    // res is the http response, including: status, headers and entity properties
    var data = res; // data is the geocoding result as parsed JSON
  })
  .catch(function(err) {
    // handle errors
  });
```
## [API](API.md)
