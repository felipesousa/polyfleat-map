# Polyfleat Map

Map Component created as example in GDG Hangouts Maceió using [Polymer](https://www.polymer-project.org/1.0/) and [LeafletJS](http://leafletjs.com/).

## Usage

1 - Install the element using Bower:

``` bash
$ bower install --save polyfleat-map 
```

2 - Import the component to your file: 

``` html
<link rel="import" href="/bower_components/polyfleat-map/polyfleat-map.html">
```

3 - Call the element: 

``` html
<polyfleat-map
    token="YOUR MAPBOX TOKEN"
    lat="YOUR LATITUDE"
    lng="YOUR LONGITUDE">
</polyfleat-map>
```

## Properties

Property  | Type        | Default   | Description
:---      |:---         |:---       |:---
`token`    | *String*    | `null`       | *You can get your token access [here](https://www.mapbox.com/studio/).
`lat`    | *Number*    | `51.050`       | *Latitude value.
`lng`    | *Number*    | `-0.09`       | *Longitude value.
`zoom`    | *Number*    | `12`       | Zoom at map.
`type`    | *Number*    | `streets`       | set your map type, that can `pirates`, `streets`, `satellite`, `light` and `dark`.

### Custom Size Map

For default, the map is 400x400 px, but, you can set the size of map, using a simple override variables, see bellow:

``` html
<style is="custom-style">
    polyfleat-map {
        --map-size-height-custom: 300px;
	--map-size-width-custom: 600px;
    }
</style>
````

## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D
