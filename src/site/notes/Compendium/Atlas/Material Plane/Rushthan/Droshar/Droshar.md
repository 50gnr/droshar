---
{"dg-publish":true,"permalink":"/compendium/atlas/material-plane/rushthan/droshar/droshar/","tags":[null],"dg-note-properties":{"type":"continent","locations":["[[Rushthan]]"],"tags":[null],"mapCalc1":0.10526315789473684,"map_height_y":3276,"map_width_x":4096,"scale_pixels":950,"scale_pixels_range":100}}
---


![Droshar.jpg\|banner](/img/user/Assets/Images/Location/Droshar.jpg)
###### Droshar
<span class="sub2">:FasEarthAmericas: Continent</span>
___

> [!quote|no-t]
>Quick description of the continent Droshar.

> [!column|flex 3]
> > [!hint]- NPC's
> > ```base
> > formulas:
> >   LinkedIndirectly: |
> >     locations.contains(this.file)
> >     || list(locations)
> >          .filter(file(value)
> >            && list(file(value).properties.locations).contains(this))
> >          .length > 0
> > 
> > properties:
> >   file.name:
> >     displayName: Name
> > 
> > views:
> >   - type: table
> >     name: This Location Only
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - locations.contains(this.file)
> > 
> >   - type: table
> >     name: Sub-Locations Included
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - formula.LinkedIndirectly
> > ```
>
>> [!example]- LOCATIONS
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Territories
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/Atlas")
> >         - locations.contains(this.file)
> > ```
>
>> [!note]- HISTORY
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Session Notes
> >     filters:
> >       and:
> >         - file.inFolder("Session Notes")
> >         - file.hasLink(this.file)
> > ```



```leaflet  
id: Droshar ### Must be unique with no spaces  
image: [Droshar.jpg](/img/user/Assets/Images/Location/Droshar.jpg) ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [3276, 4096]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 700px ### Size of the leaflet embed in px on your screen  
width: 85% ### Size of the leaflet embed in your note  
lat: 2400 ### To center the map, make this half of the map height.  
long: 1850 ### To center the map, make this half of the map width.  
minZoom: -2.5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 0.5 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -0.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.10526315789473684 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: true ### markermarker: default,2525.078315617161,1919.099644241924,,,,

```
