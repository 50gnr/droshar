---
{"dg-publish":true,"dg-path":"1-Droshar/Northern Reaches/Northern Reaches.md","permalink":"/1-droshar/northern-reaches/northern-reaches/","tags":[null],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":[null]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/default/banner.jpg)
# Northern Reaches
<span class="sub2"></span>
___

> [!quote|no-t] SUMMARY
>- **Anchor City:** [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Steeleholde/Steeleholde\|Steeleholde]]
>- **Scope:** The mountain passes, tundra forests, leyline-storm plains, and [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]].
> - **Identity:** Frontier and contested land. Villages are independent, bound by necessity against monsters and the elements. Steelholde acts as the only Imperial stronghold, though its loyalty is strained. Emberreach embodies frontier survival and suspicion of the south.
 >   
>- **Tone:** Grim, survivalist, with looming mystery (titans, ley storms, monster-haunted wilds).
> 
>- **Key Role:** The empire’s shield against northern horrors — and the most likely birthplace of rebellion.

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