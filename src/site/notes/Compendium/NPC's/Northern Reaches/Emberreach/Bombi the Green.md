---
{"dg-publish":true,"dg-path":"3-NPC's/Northern Reaches/Emberreach/Bombi the Green.md","permalink":"/3-npc-s/northern-reaches/emberreach/bombi-the-green/","tags":[["affinity/friendly"],"job/merchant","race/gnome"],"dg-note-properties":{"type":"npc","locations":["[[Drassig]]"],"tags":[["affinity/friendly"],"job/merchant","race/gnome"],"aliases":[null],"cover":"[[bombi2.png]]"}}
---


# Bombi the Green


> [!infobox|no-t right]
> ![bombi.jpg](/img/user/Assets/Images/NPC/bombi.jpg)]
> ###### Details:
> | Type | Stat |
> | ---- | ---- |
> | :FasBriefcase: Job |  Merchant |
> | :FasVenusMars: Gender | Male |
> | :FasUser: Race | Gnome |
<span class="clearfix"></span>

> [!quote|no-t]
> Profile of Bombi the Green, the male gnome NPC.

---
A travelling shrubbery salesman, Tom Bombi (LG male gnome noble), could not juxtapose the misty marshland more; with his brightly-coloured cloak and even brighter smile, Bombi is in the trade of selling shrubberies. For a mere 10 gold pieces, anyone can buy a pocket-sized shrubbery which, upon speaking its command word, will release its miniaturising magic and become a full-sized, 5-foot square garden. Bombi has heard all the tales, from the skeletal postmen, to the violation of the sacred Sepulchre of Sorrow, to the request of the ‘King’ Arfur Pendragoon to be reunited with a supposed family heirloom. He can relay these quest hooks to the player characters and explain that the bonemonger has stepped up security since the Dullovians attacked him.

## Core Handles

**Motivation (Right Now)**  
- What does this NPC want *this week*?

**Method**  
- How do they get what they want? (Charm / fear / manipulation / duty / violence)

**Relationship to PCs**
- Likes: …
- Fears / resents: …
- Wants *from* the party: …

**Secret**
- What are they hiding that would change things if revealed?

**If Cornered**
- How do they break? (Beg, lash out, bargain, flee, confess)

**Voice & Mannerisms**
- A couple quick cues: tempo, posture, pet phrase, nervous habit.

---

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
