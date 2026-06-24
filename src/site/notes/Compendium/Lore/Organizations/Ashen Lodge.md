---
{"dg-publish":true,"dg-path":"2-Lore/Organizations/Ashen Lodge.md","permalink":"/2-lore/organizations/ashen-lodge/","dg-note-properties":{"type":"organization","locations":["[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]"],"tags":null,"aliases":[null]}}
---


###### Ashen Lodge
___

> [!quote|no-t]
> “The Lodge believes survival earns purpose; sentiment is waste. Death feeds the Pyre, and the Pyre feeds the hunt.”
>  Everything beyond Emberreach is contrast.


**Lore.** The Lodge is the heart of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]. It is said the first Lodge fire was lit from the embers of the [[Compendium/Lore/Creatures/White Stag\|White Stag]]’s trail. Hunters see themselves as guardians of the cycle — to hunt is to honor, to fail is to dishonor.

**Values.** Courage, unity, respect for the kill.  

**Symbol.** A clawed hand wreathed in flame.

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