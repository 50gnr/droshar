---
{"dg-publish":true,"dg-path":"Droshar/The Esmelan Marches/The Esmelan Marches.md","permalink":"/droshar/the-esmelan-marches/the-esmelan-marches/","tags":["location/generalRegion"],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":["location/generalRegion"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### The Esmelan Marches
<span class="sub2">:FasMap: General Region</span>
___

> [!quote|no-t] SUMMARY
>Centers: Blord, Esmelar, Greenshire
>
>Identity: Fertile river valleys and farmlands, known for trade and logistics. The Marches are the breadbasket and troop-muster of the empire. The people are pragmatic, loyal to coin and land rather than crown.
>
>Tone: Bucolic with political tension; ambitious nobles jostle for position here.
>
>Key Role: Supplies both wealth and soldiers to the empire.

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