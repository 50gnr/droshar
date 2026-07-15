---
{"dg-publish":true,"dg-path":"4-Party/Sho.md","permalink":"/4-party/sho/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[ShoSlovak Trogaro]]"}}
---


# ShoSlovak Trogaro

> [!infobox|no-t right]  
> # ShoSlovak Trogaro  
> ![ShoSlovak Trogaro.png](/img/user/Assets/Images/Party/ShoSlovak%20Trogaro.png)
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Josh  
> Level | 10  
> Class | Warlock  
> Subclass | —  
> Race | Human  
> Status | Alive  
> Age | `= this.source.char_age`  
> HP | `= this.source.hp` / `= this.source.max_hp`  
> AC | `= this.source.ac`  
> Passive Perception | 1
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common 


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Overview

ShoSlovak Trogaro serves the [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] as the principal planner behind many of its operations. While others execute the mission, Sho is usually the one who has already considered a dozen ways it might fail—and prepared for each of them.

For nearly ten years he has worked alongside the Choir, helping guide political change, gathering intelligence, and ensuring every assignment begins with the best possible chance of success.

Those closest to him know that preparation is more than a habit.

For Sho...

It is survival.

---

## Description

Sho is methodical in nearly everything he does. His equipment is meticulously organized, his notes are exhaustive, and every tool has a purpose.

He rarely appears rushed.

Rarely appears surprised.

Years of planning have taught him that most disasters begin long before anyone realizes something is wrong.

Despite this discipline, Sho is approachable among his companions. He enjoys quiet evenings with [[Compendium/Party/Player Characters/Maeva the Chosen\|Maeva the Chosen]], studying old texts, discussing strange theories, or simply sharing a drink after a successful operation.

---

## Public Reputation

Within the Lotus Choir:

- operational planner
- strategist
- researcher
- meticulous organizer
- dependable under pressure

Among companions:

Sho is usually the first to ask,

> "What happens if this goes wrong?"

His plans are rarely exciting.

They simply have an irritating tendency to work.

---

## Personality

Sho believes good planning saves lives.

He is patient, analytical, and endlessly curious, particularly when confronted with ancient history, forgotten ruins, or unusual magical phenomena.

He possesses a perfectionist streak that occasionally borders on obsessive. When circumstances escape his carefully prepared plans, he often withdraws to regain his composure before returning with a clear head.

He is fiercely loyal to those he trusts, though he often expresses that loyalty through preparation rather than words.

---

## Philosophy

> _"Hope is not a strategy."_

Preparation cannot prevent every disaster.

But it can make surviving one far more likely.

---

## Relationship to [[Compendium/Party/Player Characters/Player Facing/Maeva\|Maeva]]

Maeva is Sho's closest companion.

The two have spent nearly a decade serving the Lotus Choir together and share a bond neither fully understands nor feels the need to explain.

Whether discussing impossible theories or relaxing over drinks at [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/In'nali/Sung & Gung\|Sung & Gung]], they are rarely far apart.

---

## Relationship to [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]]

The Lotus Choir gave Sho purpose when he needed it most.

They provided knowledge, direction, and a place where his unusual talents could become useful rather than feared.

He remains deeply committed to the organization, believing its work helps preserve the future he hopes to protect.

---

## Relationship to the Party

Sho helped assemble and plan many of the team's earliest operations.

Although he offers advice freely, he has little interest in commanding others.

His role is to ensure everyone understands the risks before the first step is taken.

The final decision always belongs to the team.

---

## Quotes

> "Let's make the mistake on paper instead."

> "There is always another contingency."

> "Give me ten minutes."

> "That wasn't supposed to happen."

> "We'll need a better plan."

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