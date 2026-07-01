---
{"dg-publish":true,"dg-path":"2-Lore/Organizations/Long Shadow.md","permalink":"/2-lore/organizations/long-shadow/","tags":[null],"dg-note-properties":{"type":"organization","locations":["[[Droshar]]"],"tags":[null],"aliases":["Empire","The Empire"]}}
---


# Long Shadow


> [!quote|no-t]
>![embed.jpg\|right wm-sm](/img/user/Assets/Images/default/embed.jpg)**Lore.** The [[Compendium/NPC's/Salren/Kael Vorrath\|Emperor]]’s reach extends like frost across the land, inevitable and consuming. In [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]], the Empire is present in whispers, gold, and promises of safety.
>
>**Values.** Dominion, wealth, order under imperial will.  
>
>**Symbol.** A golden sun above a crown.

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