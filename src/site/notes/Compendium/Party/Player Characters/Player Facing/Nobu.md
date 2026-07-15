---
{"dg-publish":true,"dg-path":"4-Party/Nobu.md","permalink":"/4-party/nobu/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Nobumasa Shigure]]"}}
---


# Nobumasa Shigure

> [!infobox|no-t right]  
> # Nobumasa Shigure  
> ![Nobumasa Shigure.png](/img/user/Assets/Images/Party/Nobumasa%20Shigure.png) 
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Jasen  
> Level | 10  
> Class | Rogue  
> Subclass | —  
> Race | Hanataka Tengu  
> Status | Alive  
> Age | `= this.source.char_age`  
> HP | `= this.source.hp` / `= this.source.max_hp`  
> AC | `= this.source.ac`  
> Passive Perception | `= this.source.pasperc`
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common 



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Overview

Nobu Shigure serves the Lotus Choir as a Cleaner, specializing in discreetly resolving problems that cannot be left behind. Whether protecting an operative's identity, recovering sensitive information, or ensuring a mission truly ends, he approaches every assignment with quiet professionalism and unwavering discipline.

Raised within the Shigure Compound, Nobu has spent most of his life surrounded by generations of Choir operatives. Duty comes naturally to him, but so does hospitality. Away from assignments, he is an easy companion—welcoming, dependable, and rarely one to seek the spotlight.

## Description

Nobu is a Hanataka Tengu whose calm demeanor often puts others at ease. He speaks thoughtfully rather than often, preferring to observe before offering an opinion. Years of training have made his movements economical and deliberate, whether preparing tea, maintaining his equipment, or carrying out his work.

During quieter moments, he can often be found idly shuffling a well-worn deck of playing cards or practicing the occasional bit of sleight of hand. While hardly a performer, he enjoys using the odd trick to entertain a passing child or lighten the mood during long stretches of travel.

## Public Reputation

Within the Lotus Choir:

- dependable Cleaner
- disciplined operative
- observant
- patient
- trusted to finish difficult assignments

Among companions:

Nobu is easy to live and travel with.

He keeps to a routine, quietly helps where needed, and rarely leaves work for someone else to finish. After enough years together, his companions have learned that if Nobu notices something, it is usually worth paying attention.

## Personality

Nobu is reserved without being distant. He values competence, honesty, and preparation, but carries little interest in proving himself. He is patient with those willing to learn and has a quiet fondness for children, whose carefree curiosity contrasts with the structured upbringing he experienced.

He believes every person deserves respect until they give reason otherwise, and every companion deserves to come home if they can.

## Philosophy

**"Do the small things well, and the difficult things become easier."**

Nobu believes that discipline is built through ordinary habits rather than extraordinary moments. A maintained weapon, a packed bag, a shared meal, or a few extra minutes spent preparing often matter more than talent alone.

Duty gives his work purpose, but kindness reminds him why the work matters.

## Relationship to Maki Maki

Nobu has worked alongside Maki Maki more than anyone else on the team. As a Cleaner, his assignments have a habit of intersecting with the minister's work often enough that the two have developed an easy professional rapport.

Experience has also taught Nobu that when Maki's name appears in a briefing, it is wise to leave a little extra room in the schedule.

## Relationship to the Lotus Choir

Born into a family that has served the Choir for generations, Nobu has never known another life. He believes deeply in its purpose and trusts the judgment of those who lead it, carrying out his duties with quiet conviction.

Though steadfast in that duty, he never forgets that every assignment involves people, and he carries the weight of difficult decisions long after the mission is complete.

## Relationship to the Party

Nobu has worked alongside the group since its formation nearly a decade ago. While he forms few dramatic rivalries or friendships, he is a steady presence others have come to rely upon.

Whether sharing a quiet watch, making tea during a long journey, or simply offering a listening ear, Nobu is often the sort of companion whose support is felt more than announced.

## Quotes

_"The mission isn't over until everyone gets home."_

_"There's usually a simpler solution. We just haven't noticed it yet."_

_"A clean blade begins with clean hands."_

_"Children are much harder to fool than adults."_

_"Tea first. Decisions after."_

```ability
abilities:
  strength: 10
  dexterity: 10
  constitution: 10
  intelligence: 10
  wisdom: 10
  charisma: 10

proficiencies:
  - intelligence
  - wisdom
```

<br>

```skills
proficiencies:
  - arcana
  - deception
  - history
  - insight
  - investigation
```


</div></div>


---

## Known Items




| Known Items                                                                   |
| ----------------------------------------------------------------------------- |
| [[Compendium/Lore/Objects/The Shigure Kusarigama\|The Shigure Kusarigama]] |

{ .block-language-dataview}


---

> [!column|flex 3]
>> [!important]- QUESTS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected Quests
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Party/Quests")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
>> ```
>
>> [!example]- GROUPS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected Groups
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Groups")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
>> ```
>
>> [!note]- HISTORY
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Session Notes
>>     filters:
>>       and:
>>         - file.inFolder("Session Notes")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
>> ```