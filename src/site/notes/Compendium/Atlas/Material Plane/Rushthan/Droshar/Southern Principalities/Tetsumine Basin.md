---
{"dg-publish":true,"dg-path":"1-Droshar/Southern Principalities/Tetsumine Basin.md","permalink":"/1-droshar/southern-principalities/tetsumine-basin/","tags":["location","region","lake","mountains","raiko"],"dg-note-properties":{"type":"place","locations":["[Southern Principalities]]"],"tags":["location","region","lake","mountains","raiko"],"aliases":["Tetsumine Basin"],"cover":"[[Tetsumine Basin.png\|Tetsumine Basin.png](/img/user/Compendium/Atlas/Material%20Plane/Rushthan/Droshar/Southern%20Principalities/Southern%20Principalities.md)"}}
---


# Tetsumine Basin

> "The storm never truly leaves."

> [!infobox|no-t right]
> # Tetsumine Basin
> ![[Tetsumine Basin.png\|Tetsumine Basin.png]]
> ###### Basic Information
> Type | Detail
> ---|---
> Region | Western Mountains
> Largest Settlement | [[Ironspire\|Ironspire]]
> Associated Kaiju | [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]]
> Terrain | Lake Basin
> Climate | Stormy Temperate
> Known For | Lightning Spires
>
> ###### Features
> Type | Detail
> ---|---
> Geography | Vast Mountain Lake
> Resources | Iron, Copper, Silver
> Hazard | Storm Activity
> Reputation | Hard Country


## Overview

The **Tetsumine Basin** is a vast mountain lake nestled within the western ranges of the [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Southern Principalities\|Southern Principalities]].

Hundreds of stone spires rise from the water, some little larger than a fishing boat and others towering hundreds of feet into the air. During storms these monoliths attract lightning with remarkable regularity, causing entire sections of the lake to glow with branching arcs of blue-white energy.

The basin serves as the spiritual and cultural heartland of [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]], the Herald of Storms.

---

## Geography

Tetsumine is neither a valley nor a sea.

It is a flooded basin surrounded by steep mountains and broken ridgelines.

Its defining features include:

- Vast freshwater lake
- Towering stone spires
- Deep underwater caverns
- Frequent thunderstorms
- Rich mineral deposits
- Narrow mountain passes

The lake itself is large enough that travelers often compare it to an inland sea.

---

## The Lightning Spires

The famous stone spires of Tetsumine are visible for miles.

Locals believe the formations act as natural conductors, drawing lightning from passing storms and dispersing the energy into the waters below.

Whether naturally occurring or somehow tied to [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]], scholars remain divided.

When storms roll across the basin, entire fields of spires may erupt with simultaneous lightning strikes.

The sight is considered one of the wonders of the Southern Principalities.

---

## Ironspire

The largest settlement in the region is [[Ironspire\|Ironspire]].

Built atop and between several of the largest stone formations, the city overlooks the basin and controls much of the region's mining and trade.

Its docks, bridges, and cliffside districts make it one of the most distinctive cities in the South.

---

## Legacy of the Iron Incursion

The people of Tetsumine preserve stories of an ancient conflict known as the **Iron Incursion**.

Legends speak of stone-skinned invaders, flying iron wyrms, and a desperate war fought across the basin.

According to tradition, [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]] himself intervened, granting the people the means to drive the invaders from the region.

Whether myth or history, the tale remains central to Tetsumine identity.

---

## Culture

Life in the basin is shaped by storms.

Residents are known for being:

- Practical
- Resilient
- Independent
- Direct
- Skilled craftspeople

Many families maintain traditions honoring Raiko through offerings of forged metal, bells, arrowheads, and crafted tools.

---

## Economy

The basin exports:

- Iron
- Steel
- Copper
- Silver
- Worked stone
- Tools
- Weapons

Tetsumine metalwork is respected throughout the Southern Principalities.

---

## Connection to Raiko

Among the Five Great Kaiju, none is more closely associated with a single region than [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]].

Storms across the basin are often interpreted as signs of his mood.

Periods of unusual lightning activity inevitably lead to renewed stories, speculation, and pilgrimages.

---

## Notable Locations

- [[Ironspire\|Ironspire]]
- [[Compendium/Lore/Deities/Kaiju/Raiko\|Raiko]]
- [[Stormwatch Monastery\|Stormwatch Monastery]]
- [[The Lightning Fields\|The Lightning Fields]]
- [[The Ore Roads\|The Ore Roads]]

---

## Reputation

Travelers often describe Tetsumine as:

- Beautiful
- Dangerous
- Isolated
- Honest

A common local saying states:

> "If the mountain won't kill you, the storm might."

---

## Quotes

> "The lake remembers every strike."

> "Raiko's voice is thunder."

> "The spires drink the sky."

> "Steel is forged by pressure. So are people."

---

> [!column|flex 3]
>> [!hint]- NPC's
>> ```base
>> formulas:
>>   LinkedIndirectly: |
>>     locations.contains(this.file)
>>     || list(locations)
>>          .filter(file(value)
>>            && list(file(value).properties.locations).contains(this))
>>          .length > 0
>>
>> properties:
>>   file.name:
>>     displayName: Name
>>
>> views:
>>   - type: table
>>     name: This Location Only
>>     filters:
>>       and:
>>         - file.inFolder("3-NPC's")
>>         - locations.contains(this.file)
>>
>>   - type: table
>>     name: Sub-Locations Included
>>     filters:
>>       and:
>>         - file.inFolder("3-NPC's")
>>         - formula.LinkedIndirectly
>> ```
>
>> [!example]- LOCATIONS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Provinces
>>     filters:
>>       and:
>>         - file.inFolder("1-Droshar")
>>         - locations.contains(this.file)
>> ```
>
>> [!note]- HISTORY
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Session Notes
>>     filters:
>>       and:
>>         - file.inFolder("6-Session Notes")
>>         - file.hasLink(this.file)
>> ```