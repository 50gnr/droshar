---
{"dg-publish":true,"permalink":"/compendium/lore/events/emberreach/longnight-feast/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Longnight Feast
<span class="sub2">:RiSunFoggyFill: Seasonal Event | Midwinter</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** Born from desperation during [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]’s first brutal winters, when food was scarce, and survival uncertain. The settlers gathered what little they had and shared it.

**Customs.** Each household contributes something, no matter how small — a dried root, a strip of jerky, a flask of ale. The feast is meager but meaningful, a promise that no Emberreacher starves alone. Tales of great hunts are told to remind all why they endure.

**Tone.** Humble and communal. The PCs may be asked to provide an unusual trophy to “brighten” the feast.

|   |
|---|
|Long tables crowd Ember Square, laden not with plenty, but with enough. Bowls of stew, strips of smoked fish, and mugs of thin ale pass hand to hand. Firelight flickers on faces weary but unbroken, as hunters tell stories that rise like sparks into the night.|

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