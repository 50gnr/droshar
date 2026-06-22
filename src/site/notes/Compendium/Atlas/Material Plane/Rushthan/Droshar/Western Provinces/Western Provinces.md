---
{"dg-publish":true,"permalink":"/compendium/atlas/material-plane/rushthan/droshar/western-provinces/western-provinces/","tags":["location/generalRegion"],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":["location/generalRegion"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### Western Provinces
<span class="sub2">:FasMap: General Region</span>
___

> [!quote|no-t] SUMMARY
>- **Centers:** Salren (the capital), Drassig
   > 
>- **Identity:** Oldest Imperial lands, rich in history and tradition. Salren is the jewel of the empire and the seat of power, watching over the Bay of Hunger.
  >  
>- **Tone:** Cosmopolitan, imperial, decadent in parts.
  >  
>- **Key Role:** Heart of Imperial governance, bureaucracy, and military power.

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