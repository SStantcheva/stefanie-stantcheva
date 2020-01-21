+++
title = "Road Trips Around Cambridge"
+++

## Road Trips Around Cambridge

### Hingham to Hull

Take I-93 and Mass 3A southbound, and make a detour through Quincy Shore Dr to
get a view of the Atlantic Ocean. Then, follow Mass 3A to Hingham. Once in
Hingham, follow Gegorge Washington Blvd and Nantasket Ave all the way towards
Hull. Driving this route in the early evening is also fun. You can watch the
Moon rising from the horizon and glowing in gold.

![](./hull.jpg)

{{< initMapKitJS >}}

{{< MapKitJSMap height="300px" elementID="hull_map" >}}
let geoJSONParserDelegateHull = {
    itemForLineString: function(overlay, json) {
                overlay.style = new mapkit.Style({
                    lineWidth: 2
                });
                hull_map.addOverlay(overlay);
                hull_map.showItems(overlay);
                return overlay;
                }
}
hull_geojson = mapkit.importGeoJSON("./hull_route.geojson", geoJSONParserDelegateHull)
{{< /MapKitJSMap >}}

### Essex Costal Scenic Byway

Essex Costal Scenic Byway basically follows Mass 127 and 127A, starting at
Salem and ending in Rockport. To get to the Byway from Cambridage, take US
Route 1 northbound and then I-95 eastbound to Salem, then follow Mass 127.
The Byway passes through Gloucester, where you can detour through Atlantic Rd
to get a close view of the sea. There are many costal parks along the route,
   where you can stop and have some fun.

![](./gloucester.jpg)

{{< MapKitJSMap height="300px" elementID="essex_map" >}}
let geoJSONParserDelegateGloucester = {
    itemForLineString: function(overlay, json) {
                overlay.style = new mapkit.Style({
                    lineWidth: 2
                });
                essex_map.addOverlay(overlay);
                essex_map.showItems(overlay);
                return overlay;
                }
}
essex_geojson = mapkit.importGeoJSON("./gloucester_route.geojson", geoJSONParserDelegateGloucester)
{{< /MapKitJSMap >}}
