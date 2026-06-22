---
{"dg-publish":true,"dg-path":"2-Lore/Events/Emberreach/Ashen Vigil.md","permalink":"/2-lore/events/emberreach/ashen-vigil/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Ashen Vigil 
<span class="sub2">:FasCross: Religious Event  | Early Winter</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg) **Origins.** When the first hunters of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] died in the dawn of winter, their bodies were burned at the [[Titan’s Bones\|Titan’s Bones]], their names carved into bone so they would never be forgotten. The Ashen Vigil is the continuation of this rite — a night to remember the dead and honor the cycle.
**Customs.** At dusk, families light torches and gather at the [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Ashen Lodge/Titan's Pyre/Titan's Pyre\|Titan's Pyre]]. Hunters recite the names of all lost that year, each name pressed into the titan bone. The village stays silent until dawn, save for chanting. Children carry small bone charms to remind them that “the hunt claims all.”
**Tone.** Somber, reverent. It’s the night [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] feels most bound together. PCs may be asked to carry the ashes of a fallen hunter or carve a name themselves.

|   |
|---|
|The night air is heavy with smoke. Villagers stand in silence, torches casting long shadows on pale titan bone. One by one, names are spoken into the cold air, pressed into stone with shaking hands. The fire crackles, and the hum of something vast stirs deep within the ground.|

<span class="clearfix"></span>

> [!column|flex 3]
> > [!hint]- NPC's
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Name
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - file.hasLink(this.file)
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