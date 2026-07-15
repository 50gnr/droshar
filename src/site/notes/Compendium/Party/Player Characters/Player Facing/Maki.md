---
{"dg-publish":true,"dg-path":"4-Party/Maki.md","permalink":"/4-party/maki/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Maki Maki]]"}}
---


# Maki Maki

> [!infobox|no-t right]  
> # Maki Maki  
> ![Maki Maki.png](/img/user/Assets/Images/Party/Maki%20Maki.png) 
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Tarren  
> Level | 10  
> Class | Bard  
> Subclass | —  
> Race | Lizardman  
> Status | Alive  
> Age | `= this.source.char_age`  
> HP | `= this.source.hp` / `= this.source.max_hp`  
> AC | `= this.source.ac`  
> Passive Perception | 1
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common 



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Overview

Maki Maki serves the [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] as its public face, quietly shaping public opinion from within the highest levels of government. While most members of the Choir operate unseen, Maki's greatest strength lies in being noticed for all the right reasons.

As the Minister of Fisheries, his responsibilities carry him throughout the Southern Principalities, giving him legitimate reason to visit nearly every river, port, village, and city in the realm. Trade inspections, fisheries management, and river policy provide the perfect cover for far more discreet work on behalf of the Choir.

To the public, he is a respected minister.

To the Choir, he is one of their most valuable assets.

---

## Description

Maki is a Lizardfolk whose calm smile and measured words have become familiar throughout the Southern Principalities. He dresses with understated elegance, favoring practical robes suitable for both government chambers and muddy riverbanks.

Unlike many politicians, Maki enjoys meeting the people he represents. Whether speaking with fishermen at dawn, sharing tea with village elders, or debating policy with nobles, he carries himself with genuine warmth and curiosity.

He is rarely the loudest voice in the room.

He rarely needs to be.

---

## Public Reputation

Within the Lotus Choir:

- master political operative
- trusted negotiator
- exceptional strategist
- patient listener
- invaluable public asset

Among the people of the Southern Principalities:

Maki is simply the Minister everyone seems to like.

He remembers names.

He asks about families.

He follows up on conversations months later.

People leave interactions with Maki feeling heard.

Many never realize how much their opinions shifted while speaking with him.

---

## Personality

Maki genuinely enjoys politics.

Not because he craves authority, but because he enjoys solving problems through conversation rather than conflict.

He believes most people want the same things: safety, stability, and the chance to build a good life.

Helping them realize they already agree is often easier than convincing them they're wrong.

Though remarkably patient, Maki possesses a surprisingly quick temper. When pushed too far he may lose his composure for a brief moment before collecting himself just as quickly, almost always apologizing afterward.

He dislikes hurting ordinary people and carries genuine empathy for those caught in the wake of larger political struggles.

---

## Philosophy

> *"People rarely change their minds. They simply decide the new idea was theirs."*

Influence lasts longer than fear.

Kindness lasts longer than influence.

Whenever possible, Maki prefers both.

---

## Relationship to [[Compendium/Party/Player Characters/Player Facing/Sho\|ShoSlovak Trogaro]]

Sho is the planner.

Maki is the persuader.

Where Sho builds the operation, Maki prepares the world around it. The two have worked together long enough that many plans require little explanation between them.

---

## Relationship to [[Compendium/Party/Player Characters/Player Facing/Nobu\|Nobumasa Shigure]]

Maki's operations frequently leave Nobu responsible for ensuring every loose end is properly tied.

The two have developed an easy professional rhythm built on trust and mutual respect.

Maki often jokes that Nobu is responsible for cleaning up after him.

Nobu has never confirmed or denied the accusation.

---

## Relationship to [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]]

The Choir saw potential in Maki long before anyone else did.

They gave him opportunity, education, and purpose.

Over the years he rose from obscurity to become one of the Southern Principalities' most recognizable public officials.

He remains deeply loyal to the organization, believing its quiet guidance has preserved peace more often than history will ever record.

---

## Relationship to the Party

Among the team, Maki rarely wears the mask expected of a politician.

His companions know the person behind the public image: thoughtful, occasionally stubborn, surprisingly funny, and willing to admit when he is wrong.

Though he often helps shape the team's discussions, he has little interest in leading them.

His role is to offer perspective.

The decisions belong to everyone.

---

## Quotes

> *"Let's talk before anyone starts swinging swords."*

> *"Influence is far cheaper than rebuilding."*

> *"People remember how you made them feel long after they've forgotten what you said."*

> *"That... could have gone better."*

> *"Now, who's hungry?"*

---


</div></div>


---

## Known Items

| Known Items                                                                                          |
| ---------------------------------------------------------------------------------------------------- |
| [[Locate the Eye Ball\|Locate the Eye Ball]], [[Assets/Templates/Template-Quest\|Template-Quest]] |

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