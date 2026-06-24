---
{"dg-publish":true,"dg-path":"3-NPC's/Northern Reaches/Emberreach/Eira Mossroot.md","permalink":"/3-npc-s/northern-reaches/emberreach/eira-mossroot/","tags":["affinity/friendly","job/chef","race/shifter|elf"],"dg-note-properties":{"type":"npc","locations":["[[Mossroot's Hall]]"],"tags":["affinity/friendly","job/chef","race/shifter|elf"],"cover":"[[eira.png]]"}}
---

# Eira Mossroot

> [!infobox|no-t right]
> ![eira.png](/img/user/Assets/Images/NPC/eira.png)
> ###### Details:
> | Type | Stat |
> | ---- | ---- |
> | :FasBriefcase: Job |  Chef |
> | :FasVenusMars: Gender | Female |
> | :FasUser: Race | Shifter/Elf |
<span class="clearfix"></span>

> [!quote|no-t]
>The matron of Mossroot’s Hall, Eira is part alchemist, part cook, part village confidante. Her stews heal wounds as much as they fill bellies, and her sharp tongue spares no apprentice. Beneath her warmth lies a dangerous curiosity for biomancy.


> [!column|flex 3]
>> [!important]- QUESTS:
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Name
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Party/Quests")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
>> ```
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