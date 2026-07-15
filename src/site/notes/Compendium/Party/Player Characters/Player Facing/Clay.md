---
{"dg-publish":true,"dg-path":"4-Party/Clay.md","permalink":"/4-party/clay/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Compendium/Party/Player Characters/Clay Clay Clay]]"}}
---


# Clay

> [!infobox|no-t right]  
> # Clay  
> ![Clay.png](/img/user/Assets/Images/Party/Clay.png) 
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Wyatt  
> Level | 10  
> Class | Rogue / Barbarian  
> Subclass | —  
> Race | Hanimori  
> Status | Alive  
> Age | Old AF  
> HP | 135 / 135  
> AC | 18  
> Passive Perception | 14
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common,Thieves Can't 



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Overview

Clay Clay Clay is a Haniwa warrior who has served alongside the [[Shigure Family\|Shigure Family]] and [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] for most of his century-long existence.

He has worked with three generations of Shigure operatives, watching children become agents, agents become leaders, and leaders eventually pass their duties to those who followed. Through all of it, Clay has remained remarkably consistent.

When subtlety fails, defenses harden, or an extraction turns violent, Clay is the person sent to make certain everyone else still has a way out.

He is the contingency.

The last resort.

The one called when a problem must end immediately.

---

## Description

Clay is a towering Haniwa formed from hardened earth and weathered clay. His body carries the marks of long service: repaired cracks, worn surfaces, old impacts, and careful restoration layered across more than a hundred years of assignments.

His most recognizable possession is an enormous **ōdzutsu hand cannon**, powerful enough to break fortified positions from a distance and heavy enough to serve as a brutal club when enemies close the gap.

Despite his size and destructive equipment, Clay moves with surprising control. Years of infiltration work have taught him when to remain unseen, when to wait, and when restraint has stopped being useful.

---

## Public Reputation

Within the Lotus Choir:

- veteran operative
- emergency response specialist
- heavy weapons expert
- dependable under pressure
- trusted across generations
- difficult to permanently damage

Among companions:

Clay is direct, reliable, and rarely interested in unnecessary discussion once a decision has been made.

He may not always be the first person consulted when subtle plans are being assembled.

He is often the first person everyone looks toward when those plans collapse.

---

## Personality

Clay is all business when an assignment is active.

He prefers clear objectives, practical solutions, and decisive action. He has little patience for performances of authority, needless complexity, or plans that depend upon everyone behaving exactly as expected.

Outside the work, however, Clay can be unexpectedly peculiar.

A century of life has left him with habits, preferences, and observations that make perfect sense to him and occasionally no one else. His humor is usually delivered without warning and with such a straight face that companions are not always certain whether he intended the joke.

Clay does not speak often merely to fill silence.

When he does speak, people generally listen.

---

## Philosophy

> "If the plan still works, you don't need me yet."

Clay understands his role.

Most operations should be completed quietly.

Most problems should be resolved without violence.

Most doors should be opened rather than destroyed.

But when the quiet solution has failed, hesitation only gives the problem time to become worse.

Clay believes force is not the first answer.

It is simply an answer that must work when every other one has stopped working.

---

## Relationship to the [[Shigure Family\|Shigure Family]]

Clay has served alongside three generations of the Shigure family.

He has watched their operatives train, take assignments, raise families, grow old, and pass responsibility onward. To many younger members of the family, Clay has always been part of the compound—less a visitor than one of its permanent foundations.

He remembers the Shigures differently from how they remember themselves.

Children he once watched train eventually became the people giving him orders.

He rarely comments upon this unless asked.

---

## Relationship to [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]]

The Lotus Choir has provided Clay with duty, continuity, and purpose for most of his known life.

He is not especially interested in the organization's politics. Leaders change. Methods evolve. Arguments repeat under different names.

The work remains.

Clay judges the Choir by the assignments placed before him and the people standing beside him when those assignments become difficult.

---

## Relationship to the Party

Clay has served with the current team since its formation.

His companions know him as their final layer of protection: the distant silhouette on a rooftop, the heavy footsteps behind an extraction, or the sudden report of an ōdzutsu when a situation has crossed the point of negotiation.

He expects the others to handle their responsibilities.

They trust that when something survives long enough to reach Clay...

it will not survive much longer.

---

## The Ōdzutsu

Clay's oversized hand cannon functions as both firearm and close-quarters weapon.

At range, it provides overwhelming force against fortified positions, dangerous targets, or groups that have become impossible to contain.

At close quarters, Clay simply reverses his grip.

The reinforced barrel has ended nearly as many fights as the shot fired through it.

Clay maintains the weapon personally and allows very few people to handle it.

---

## Quotes

> "Still quiet? Then everything is fine."

> "Move away from the door."

> "That was the subtle option."

> "It has worked for a hundred years."

> "You had a plan. Now you have me."

---


</div></div>


---

## Known Items

| Known Items |
| ----------- |
| \-          |

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