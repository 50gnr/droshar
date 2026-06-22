---
{"dg-publish":true,"dg-path":"2-Lore/Events/Emberreach/Greenmark.md","permalink":"/2-lore/events/emberreach/greenmark/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Greenmark
<span class="sub2">:RiSunFoggyFill: Seasonal Event | First Thaw</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/embed.jpg)**Origins.** When [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]’s first settlers survived their first spring, they marked their homes with moss and green paint, hoping to invite life back after winter’s grip.

**Customs.** Families smear moss or green paint over doorframes. Hunters wear willow branches in their hair. Apprentices are often sent to fetch the “first bloom” — a flower that appears deep in the thawing woods — as a test of courage.

**Tone.** Joyous, muddy, chaotic. Children dash about marking each other with green hands. PCs may get dragged into a “first bloom” quest.

|   |
|---|
|The village bursts into color. Moss and green paint streak doorways, children chase each other with green-stained hands, and laughter rings through thawing air. Hunters stride through the square with willow branches in their hair, daring apprentices to bring back the first bloom.|

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