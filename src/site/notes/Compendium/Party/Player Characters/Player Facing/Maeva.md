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
> Age | `= this.source.char_age`  
> HP | `= this.source.hp` / `= this.source.max_hp`  
> AC | `= this.source.ac`  
> Passive Perception | `= this.source.pasperc`
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common 

## Overview


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



## Description

As a Changeling, Maeva rarely maintains one appearance for long.

Some disguises are practical.

Others are beautiful.

Some exist only because they make a conversation easier.

Regardless of her appearance, she carries herself with quiet confidence and deliberate grace.

Those meeting her for the first time often leave believing they met exactly the person they expected.

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