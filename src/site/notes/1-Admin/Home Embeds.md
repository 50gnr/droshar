---
{"dg-publish":true,"permalink":"/1-admin/home-embeds/","dg-note-properties":{}}
---



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

