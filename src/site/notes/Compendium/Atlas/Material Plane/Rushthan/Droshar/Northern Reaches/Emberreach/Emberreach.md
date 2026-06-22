---
{"dg-publish":true,"dg-path":"Droshar/Northern Reaches/Emberreach/Emberreach.md","permalink":"/droshar/northern-reaches/emberreach/emberreach/","tags":[null],"dg-note-properties":{"type":"locale","locations":["[[Northern Reaches]]"],"tags":[null],"mapCalc1":"NaN","map_height_y":5376,"map_width_x":9472}}
---


![Emberreach.webp\|banner](/img/user/Assets/Images/Location/Emberreach.webp)
###### Emberreach
<span class="sub2"></span>
___

> [!quote|no-t] SUMMARY
>Where the winters last nearly nine months and the forests whisper with the echoes of titans, there lies Emberreach — a village of hunters, smiths, mystics, and storytellers. Here, life is carved from frost and fire, where survival is never guaranteed, and glory is measured in the trophies you bring home.
>
>The people of Emberreach are not farmers, nor merchants, nor nobles. They are hunters — of beasts, of legends, of the very land itself. When outsiders think of the North, they think of hardship; when Emberreachers speak of it, they speak of honor, ash, and the eternal hunt.
>
>[[Prep/Northern Reaches C1/Emberreach Events\|Emberreach Events]]


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
> >     name: Landmarks
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
id: MapCalcExample ### Must be unique with no spaces  
image: [Emberreach.webp](/img/user/Assets/Images/Location/Emberreach.webp) ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [5376, 9472]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 700 ### Size of the leaflet embed in px on your screen  
width: 95% ### Size of the leaflet embed in your note  
lat:  2688  ### To center the map, make this half of the map height.  
long: 4736 ### To center the map, make this half of the map width.  
minZoom: -3.5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: -1.5 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -3.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### marker
```
