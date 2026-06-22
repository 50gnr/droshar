---
{"dg-publish":true,"dg-path":"4-Party/Clay.md","permalink":"/4-party/clay/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Clay Clay Clay]]"}}
---

a
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
> HP | 50 / 71  
> AC | 80  
> Passive Perception | 13
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Celestial,Common,Dwarvish 

## Overview


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Description

This is the persons description. 


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