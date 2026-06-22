---
{"dg-publish":true,"dg-path":"Droshar/Desert Kingdoms/Desert Kingdoms.md","permalink":"/droshar/desert-kingdoms/desert-kingdoms/","tags":["location/generalRegion"],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":["location/generalRegion"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### Desert Kingdoms
<span class="sub2">:FasMap: General Region</span>
___

> [!quote|no-t] SUMMARY
>- **Centers:** Dathmyr, Kubaru
    >
>- **Identity:** Harsh deserts and caravan cities, marked by oases, ancient ruins, and trade with southern continents. A culture of resilience, hospitality, and blood-oaths.
  >  
>- **Tone:** Exotic, ancient, mystical.
  >  
>- **Key Role:** Source of trade wealth, rare resources, and ancient magical secrets.

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
> >     name: Provinces
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