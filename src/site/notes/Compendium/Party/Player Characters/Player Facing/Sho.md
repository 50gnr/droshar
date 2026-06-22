---
{"dg-publish":true,"dg-path":"4-Party/Player Facing/Sho.md","permalink":"/4-party/player-facing/sho/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[ShoSlovak Trogaro]]"}}
---


# ShoSlovak Trogaro

> [!infobox|no-t right]  
> # ShoSlovak Trogaro  
> ![ShoSlovak Trogaro.jpeg](/img/user/Assets/Images/Party/ShoSlovak%20Trogaro.jpeg) 
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
> Affiliation |  
> Languages | Common 

## Overview


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Description

This is the persons description. 


</div></div>


---

## Known Items

| Known Items                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- |
| [[Locate the Eye Ball\|Locate the Eye Ball]], [[z_Templates/World Builder Templates/Template-Quest\|Template-Quest]] |

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