---
{"dg-publish":true,"dg-path":"1-Droshar/Southern Principalities/Bardune.md","permalink":"/1-droshar/southern-principalities/bardune/","tags":["location/city"],"dg-note-properties":{"type":"locale","locations":["[[Southern Principalities]]"],"tags":["location/city"]}}
---


![bardune.png](/img/user/Assets/Maps/Bardune/bardune.png)
# Bardune


> [!quote|no-t] SUMMARY
> “They shout at the mountain until it answers. One day it will.”

**Type:** Lake City, Forest-Buried  
**Population:** ~18–22k  
**Dominant Aesthetic:** Cedar, moss, lacquered wood, stone lanterns half-swallowed by roots  
**Primary Spirits:** Lake yokai, forest guardians, ancestral shades
**Governor:** [[Compendium/NPC's/Southern Principalities/Seiha Riverlily\|Seiha Riverlily]]

## Identity

Bardune sits on the shores of a deep, cold lake hidden beneath an ancient forest canopy. The city was _grown_, not planned—built outward from shrines, docks, and spirit-bound clearings. Buildings lean, streets curve, and fog is considered a sign of good fortune.

Bardune’s people believe the land remembers everything.

## Philosophy

> **“The land listens. Speak softly.”**

Bardunese culture centers on **appeasement, balance, and memory**. Spirits are not ruled, only negotiated with. Progress is acceptable only if it does not disturb what sleeps beneath the lake or within the roots.

Change is slow by design.

## Governance

- **The Lake Council** – elders, shrine-keepers, and hereditary wardens
    
- Decisions require **ritual consensus**, not votes
    
- Outsiders find Bardune maddeningly indirect
    

## Economy

- Spirit-lacquered crafts
    
- Lake pearls, rare fish, medicinal fungi
    
- Whisperwood instruments and talismans
    

## View of In’nali

Bardune sees In’nali as **reckless but necessary**—people who _force answers_ instead of waiting for them.


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
> >         - file.inFolder("Session Notes/C2 Southern Principalities/Recap")
> >         - file.hasLink(this.file)
> > ```