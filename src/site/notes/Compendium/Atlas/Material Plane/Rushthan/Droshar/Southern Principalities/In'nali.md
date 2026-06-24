---
{"dg-publish":true,"dg-path":"1-Droshar/Southern Principalities/In'nali.md","permalink":"/1-droshar/southern-principalities/in-nali/","tags":["location/city"],"dg-note-properties":{"type":"locale","locations":["[[Southern Principalities]]"],"tags":["location/city"]}}
---


![in'nali.png](/img/user/Assets/Maps/In'nali/in'nali.png)
# In'nali


> [!quote|no-t] SUMMARY
> “They pray the lake stays calm. We ensure the mountain does.”

**Type:** Plateau City, Cliff-Crowned  
**Population:** ~25–30k  
**Dominant Aesthetic:** Stone terraces, wind banners, hanging bridges, sun-bleached bamboo  
**Primary Spirits:** Sky yokai, ancestral giants, sealed colossi
**Steward:** [[Compendium/NPC's/Southern Principalities/Aketsu Blackwing\|Aketsu Blackwing]]

## Identity

In’nali is built atop a massive plateau, its cliffs carved into stepped districts connected by lifts, stairs, and switchback roads. From below it appears unreachable; from above it feels exposed—always in the wind, always watched by the sky.

In’nali believes survival comes from **commanding position**, not concealment.

## Philosophy

> **“That which sleeps must be guarded.”**

In’nali culture emphasizes **vigilance, strength, and responsibility**. Spirits are dangerous forces to be bound, watched, or—if necessary—awakened _under strict conditions_.

Inaction is considered a moral failure.

## Governance

- **The High Circles** – military stewards, ritual engineers, and oathbound houses
    
- Authority is earned through **service and sacrifice**
    
- Decisions are fast, recorded, and binding
    

## Economy

- Stonecraft, wind-driven mills
    
- Kaiju-adjacent alloys and reinforced ceramics
    
- Caravans and tolls from plateau roads
    

## View of Bardune

In’nali sees Bardune as **naïve custodians**—keepers of stories who mistake patience for wisdom.



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