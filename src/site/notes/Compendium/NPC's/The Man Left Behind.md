---
{"dg-publish":true,"dg-path":"3-NPC's/The Man Left Behind.md","permalink":"/3-npc-s/the-man-left-behind/","tags":["npc","lotus-choir","former-operative","rival"],"dg-note-properties":{"type":"npc","locations":["[[Southern Principalities]]"],"tags":["npc","lotus-choir","former-operative","rival"],"aliases":["The Man Left Behind"],"cover":"[[Image Name.png]]"}}
---


> [!infobox|no-t right]
> ![portrait.jpg](/img/user/Assets/Images/default/portrait.jpg)
> ###### Details:
> | Type | Stat |
> | ---- | ---- |
> | :FasBriefcase: Job |   |
> | :FasVenusMars: Gender |  |
> | :FasUser: Race |  |
<span class="clearfix"></span>

# The Man Left Behind

## Overview

A former Lotus Choir operative who once served alongside [[Compendium/Party/Player Characters/Nobumasa Shigure\|Nobu]] early in his career.

During an operation, he chose what he believed was the ethical course of action, even though it placed the objective at risk.

Nobu chose the mission.

The objective was completed.

The other operative was left behind and taken into custody.

---

## Relationship to Nobu

Before they parted, he swore Nobu would one day answer for his choice.

Nobu does not know where he is now.

Whether he escaped, was released, defected, or disappeared remains unknown.

---

# Hidden Data

## Presentation Notes

- Personal, not theatrical.
- Believes Nobu made the wrong choice.
- Not necessarily evil.
- May still believe he was the one who acted with honor.
- Should feel like consequence, not a random enemy.



## Truth

His current status is undecided.

Possible uses:

- Returned rival
- Enemy informant
- Captive needing rescue
- Anti-Choir operative
- Someone who has built a life around hating Nobu

## Story Use

This NPC exists to challenge Nobu's certainty.

The question is not whether Nobu completed the mission.

He did.

The question is what kind of person that choice made him.

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



