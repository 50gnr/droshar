---
{"dg-publish":true,"dg-path":"4-Party/Player Facing/Nobu.md","permalink":"/4-party/player-facing/nobu/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[Nobumasa Shigure]]"}}
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

## Overview


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Description

This is the persons description. 


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