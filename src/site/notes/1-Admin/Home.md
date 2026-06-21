---
{"dg-publish":true,"permalink":"/1-admin/home/","tags":["gardenEntry"],"dg-note-properties":{"obsidianUIMode":"preview"}}
---





> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🧙Party),
> option(2, 📚Session Journals),
> option(3, ➕Create New),
> option(4, 🪶NPCs),
> option(5, 📈Locations),
> option(6, 📈Recently Modified),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h1 clean

</div>


# Party

```base
properties:
  property.char_race:
    displayName: Race
  property.char_gender:
    displayName: Gender
  property.char_status:
    displayName: Status
  property.char_class:
    displayName: Class
  property.char_age:
    displayName: Age
  property.char_items:
    displayName: Inventory
  file.name:
    displayName: Character Name
  property.Player:
    displayName: Player Name
  property.level:
    displayName: Level
views:
  - type: table
    name: Party Members
    filters:
      and:
        - file.tags.contains("Category/Player")
        - file.folder == "Compendium/Party/Player Characters"
    order:
      - file.name
      - property.Player
      - property.char_race
      - property.char_gender
      - property.level
      - property.char_status
      - property.char_class
      - property.char_age
      - property.char_items
    sort:
      - property: file.name
        direction: ASC

    columnSize:
      file.name: 185
      property.Player: 88
      property.level: 43
      property.char_status: 143
      property.char_class: 145
      property.char_age: 165

```


</div></div>

> >
> > >[!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h clean

</div>


# Session Journals

```base
views:
  - type: table
    name: Session Journals
    filters:
      and:
        - file.folder == "Session Notes"
    order:
      - file.name
      - Status
      - players
    sort:
      - column: file.name
        direction: DESC
    limit: 6
```




</div></div>

> >
> > >[!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h1 clean

</div>


# Create New

### Player Elements

`BUTTON[pc]`

`BUTTON[note]` 

---
### World Elements

`BUTTON[plane]` 

 `BUTTON[realm]` 

`BUTTON[continent]` 

 `BUTTON[territory]` 
 
 `BUTTON[province]` 
 
 `BUTTON[locale]`  - Places where people live - Cities, Towns, Villages, Hamlets, Encampment, Keeps, Fortresses, Strongholds.

 
 `BUTTON[landmark]` - Places that can be explored (dungeons, ruins, etc).

`BUTTON[npc]`  

`BUTTON[org]` - Groups of people and power - religious, cults, guilds, military

`BUTTON[quest]`  

`BUTTON[object]`  

---

#### Mechanical Elements

`BUTTON[object]`

`BUTTON[creature]`


</div></div>

> >
> > > [!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h1 clean

</div>


# NPC's


 ```base

 views:
   - type: cards
     name: Cards
     filters:
       and:
         - file.inFolder("Compendium/NPC's")
         - file.hasLink("Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Southern Principalities")
     order:
       - file.name
     image: note.cover
     imageAspectRatio: 1.3
     imageFit: "vertical"
     cardSize: 200

   - type: table
     name: List
     filters:
       and:
       - file.hasLink("Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Southern Principalities")
       - file.inFolder("Compendium/NPC's")
     order:
       - file.name
 ```
 ---



</div></div>

> > 
> > > [!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h1 clean

</div>


# Locations

 ```base

 properties:
   file.name:
     displayName: Name
     
 views:
   - type: cards
     name: Cards
     filters:
       and:
         - file.inFolder("Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities")
     order:
       - file.name

   - type: table
     name: List
     filters:
       and:
         - file.inFolder("Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities")
     order:
       - file.name
       - type
 ```
 ---



</div></div>

> > 
> > > [!div-m|no-title]
> > > 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# no-h1 clean

</div>


# Recently Modified

```base
views:
  - type: table
    name: Recently Modified - All
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
      - obsidianUIMode
    columnSize:
      file.name: 177
      property.MyContainer: 189
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 170
    sort:
      - column: file.mtime
        direction: DESC
      - column: file.ctime
        direction: ASC
      - column: file.folder
        direction: DESC
      - column: property.MyCategory
        direction: ASC
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Regions
    filters:
      and:
        - file.folder == "2-World/Regions"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Hubs
    filters:
      and:
        - file.folder == "2-World/Hubs"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: file.name
        direction: DESC
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Places
    filters:
      and:
        - file.folder == "2-World/Places"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: file.name
        direction: DESC
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Places of Interest
    filters:
      and:
        - file.folder == "2-World/Points of Interest"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: People
    filters:
      and:
        - file.folder == "2-World/People"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 154
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Groups
    filters:
      and:
        - file.folder == "2-World/Groups"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: file.ctime
        direction: ASC
      - column: file.name
        direction: ASC
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Quests
    filters:
      and:
        - file.folder == "2-World/Quests"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: property.Status
        direction: DESC
    limit: 10
  - type: table
    name: Session Journals
    filters:
      and:
        - file.folder == "1-Session Journals"
    order:
      - file.name
      - MyContainer
      - MyCategory
      - file.folder
      - file.ctime
      - file.mtime
    columnSize:
      file.name: 177
      property.MyContainer: 244
      property.MyCategory: 175
      file.folder: 273
      file.ctime: 208
    sort:
      - column: file.name
        direction: ASC
      - column: property.Status
        direction: DESC
    limit: 10

```


</div></div>




```leaflet  
id: Droshar ### Must be unique with no spaces  
image: [Droshar.jpg](/img/user/Assets/Images/Location/Droshar.jpg) ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [3276, 4096]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 700px ### Size of the leaflet embed in px on your screen  
width: 85% ### Size of the leaflet embed in your note  
lat: 488 ### To center the map, make this half of the map height.  
long: 2680 ### To center the map, make this half of the map width.  
minZoom: -2.5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 0.5 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -0.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.10526315789473684 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: true ### markermarker: default,2525.078315617161,1919.099644241924,,,,

```