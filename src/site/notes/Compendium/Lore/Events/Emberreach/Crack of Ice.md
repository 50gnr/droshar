---
{"dg-publish":true,"permalink":"/compendium/lore/events/emberreach/crack-of-ice/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Crack of Ice
<span class="sub2">:RiSunFoggyFill: Seasonal Event | Late Winter</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** The frozen river is [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]’s lifeline, and when its ice first cracks in spring, it heralds survival. In old tales, the crack was the voice of river spirits freed from winter’s grip.

**Customs.** When the first crack thunders, bells ring across the village. Children throw flowers, carved charms, or tokens into the river to appease the spirits. Hunters interpret the tone of the crack — sharp, soft, late, or early — as omens for the coming season.

**Tone.** Hopeful but edged with superstition. A bad crack breeds unease. PCs might be asked to follow strange signs near the river.

|   |
|---|
|The ice splits with a thunderous crack, echoing across the glade like a god’s voice. Bells ring from the square, and villagers rush to the riverbank, tossing flowers and charms into the dark waters. The air is alive with cheers — and whispers of what the sound portends.|


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