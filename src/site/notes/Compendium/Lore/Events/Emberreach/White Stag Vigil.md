---
{"dg-publish":true,"dg-path":"2-Lore/Events/Emberreach/White Stag Vigil.md","permalink":"/2-lore/events/emberreach/white-stag-vigil/","tags":["event/religious"],"dg-note-properties":{"type":"event","tags":["event/religious"]}}
---


###### White Stag Vigil
<span class="sub2">:FasCross: Religious Event | Late Summer</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** The White Stag, said to have led settlers to [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]], is seen as a sacred omen. Sightings are rare, and always portentous.

**Customs.** For a week, villagers hang white banners and keep watch at night. Hunters may set out in pursuit, though the stag is rarely caught. Legends say those who kill it doom [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]], while those who follow it find destiny.

**Tone.** Mysterious, charged with omen. PCs might be asked to protect, pursue, or interpret its meaning.

|   |
|---|
|White banners flutter from rooftops as the village falls into hushed anticipation. At night, watchers line the palisade, whispering of glowing eyes in the treeline. Somewhere out there, they say, the White Stag waits.|

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