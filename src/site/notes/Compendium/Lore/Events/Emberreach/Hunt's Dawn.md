---
{"dg-publish":true,"permalink":"/compendium/lore/events/emberreach/hunt-s-dawn/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Hunt's Dawn
<span class="sub2">:RiSunFoggyFill: Seasonal Event | Spring Equinox</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** The equinox marks the balance of night and day — and [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] sees it as the start of the hunting season. It is also the traditional graduation rite for apprentices.

**Customs.** Lodge apprentices undertake their first sanctioned monster hunt. Those who succeed carve their sigil into bone. Those who fail return in shame, or not at all.

**Tone.** Sacred and perilous. A PC’s first hunt could coincide with this festival.

|   |
|---|
|The fire in the Lodge roars higher than usual, its heat searing. Apprentices stand in a line, steel and bone sigils in hand, as Weyland’s voice cuts through the hall. “The Hunt’s Dawn rises. Go forth — and return worthy.”.|


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