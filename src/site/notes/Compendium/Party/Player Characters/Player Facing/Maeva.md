---
{"dg-publish":true,"dg-path":"4-Party/Maeva.md","permalink":"/4-party/maeva/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Maeva the Chosen]]"}}
---


# Maeva the Chosen

> [!infobox|no-t right]  
> # Maeva the Chosen  
> ![Maeva the Chosen.png](/img/user/Assets/Images/Party/Maeva%20the%20Chosen.png) 
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Louis  
> Level | 10  
> Class | Cleric  
> Subclass | —  
> Race | Changeling  
> Status | Alive  
> Languages | Common 

## Overview


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Overview

Lady Maeva serves the [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] as an infiltration specialist, moving effortlessly between disguises, identities, and social circles.

A wardrobe exists for every occasion.

A conversation exists for every situation.

To those who know her well, however, the performance ends. Beneath every face lies someone remarkably comfortable with simply existing in the present.

---

## Description

As a Changeling, Maeva rarely maintains one appearance for long.

Some disguises are practical.

Others are beautiful.

Some exist only because they make a conversation easier.

Regardless of her appearance, she carries herself with quiet confidence and deliberate grace.

Those meeting her for the first time often leave believing they met exactly the person they expected.

---

## Public Reputation

Within the Lotus Choir:

- exceptional infiltrator
- consummate professional
- adaptable
- dependable
- difficult to truly know

Among companions:

Maeva is polite.

Helpful.

Pleasant company.

She simply avoids becoming dependent upon anyone.

---

## Personality

Maeva believes every situation deserves the right face.

The right words.

The right approach.

She rarely takes offense and seldom clings to resentment.

If someone doesn't wish her company...

She simply finds somewhere else to be.

Work remains work.

Friendship is welcomed, never expected.

---

## Philosophy

> "People change. Why shouldn't I?"

Maeva embraces change rather than resisting it.

Identity is a tool.

The present is what matters.

Yesterday cannot be altered.

Tomorrow has not yet arrived.

---

## Relationship to [[Compendium/Party/Player Characters/Player Facing/Sho\|Sho]]

Sho is the closest thing Maeva considers family.

The two have served together for many years and share an understanding that few others could truly appreciate.

When off duty, they're often found sharing a quiet drink together.

---

## Relationship to [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]]

Maeva has served the Lotus Choir for nearly a decade.

The Choir gave her purpose when she needed one.

In return...

She has become one of its most reliable operatives.

---

## Relationship to the Party

Maeva has worked alongside the team since its formation.

She values competence above bravado and trusts actions more than promises.

Though rarely openly sentimental, she quietly watches over those she considers her companions.

## Quotes

> "There is always another face."

> "People tell you exactly who they are if you let them talk."

> "Attachment is a choice."

> "Every conversation begins long before the first word."

> "We're here to finish the mission."

---


</div></div>


---

## Known Items

| Known Items                                |
| ------------------------------------------ |
| [[The Chosens Shield\|The Chosens Shield]] |

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