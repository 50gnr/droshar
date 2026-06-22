---
{"dg-publish":true,"permalink":"/compendium/lore/events/emberreach/emberfall-rite/","tags":["event/religious"],"dg-note-properties":{"type":"event","tags":["event/religious"]}}
---


###### Emberfall Rite
<span class="sub2">:FasCross: Religious Event | Late Autumn</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** Before winter descends, [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] casts weakness into the flames — both symbolic and practical. Broken tools, cracked weapons, and ruined charms are burned at the [[Titan’s Pyre\|Titan’s Pyre]].

**Customs.** Each family contributes one thing to burn. Hunters often toss in broken arrows or dulled knives. Apprentices are expected to give something personal — a childhood toy, a worn-out tool — to mark their step into the harsh season.

**Tone.** Reflective, ritualistic. PCs can use this to show personal growth.

|   |
|---|
|The flames of the Pyre roar high as villagers file past, each casting something into the fire: a cracked tool, a dulled blade, a child’s broken toy. Sparks leap skyward as the wind howls, carrying weakness away into the long night.|


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