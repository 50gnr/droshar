---
{"dg-publish":true,"dg-path":"2-Lore/Events/Emberreach/Ember Games.md","permalink":"/2-lore/events/emberreach/ember-games/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


###### Ember Games
<span class="sub2">:RiSunFoggyFill: Seasonal Event | Midsummer</span>
___

> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/default/embed.jpg)**Origins.** A celebration of strength and skill, the Ember Games began as a way to test hunters in contests without risking death.

**Customs.** Archery, wrestling, axe-throwing, endurance runs. Wagers are common, and rivalries flare hot. The Lodge views it as practice — the villagers see it as festival.

**Tone.** Loud, competitive, spirited. PCs may be challenged, cheered, or humiliated.

  

|   |
|---|
|Cheers erupt across Ember Square as axes thud into targets and wrestlers grapple in the dirt. Torches blaze, ale flows, and the air rings with laughter and shouted wagers. Hunters watch from the sidelines, eyes sharp even in celebration.|

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