---
{"dg-publish":true,"permalink":"/compendium/lore/events/emberreach/hunt-s-feast/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Hunt's Feast
<span class="sub2">:RiSunFoggyFill: Seasonal Event | Early Autumn</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** When crops are harvested and the last great hunts complete, [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] feasts to give thanks.

**Customs.** Hunters present trophies in the square. Families share preserved meats, roasted beasts, and rare summer ales. Rival bands compare kills, and apprentices show their worth.

**Tone.** Celebratory, competitive. PCs can shine — or be shamed.

|   |
|---|
|The square bursts with fire and music. Antlers, claws, and fangs hang from posts, each trophy a story told over mugs of spiced ale. Villagers dance in circles, stamping feet echoing the beat of drums as hunters laugh and boast of the kills that filled their tables.|

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