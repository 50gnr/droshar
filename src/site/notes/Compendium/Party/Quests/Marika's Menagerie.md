---
{"dg-publish":true,"dg-path":"2-Lore/Rumors/Marika's Menagerie.md","permalink":"/2-lore/rumors/marika-s-menagerie/","tags":["Category/Quest","quest","rumor"],"dg-note-properties":{"type":"quest","tags":["Category/Quest","quest","rumor"],"MyContainer":["[[Southern Principalities (41116)]]"],"MyCategory":null,"quest_type":"rumor","questObtained":null,"questStatus":"Rumor","questGiver":null,"questLocationObtained":null,"questSessionObtained":null,"questNotes":null,"questLootAvail":null,"questLookEarned":null,"cover":"[[Marika's Menagerie.png]]","obsidianUIMode":"preview"}}
---


# Marika's Menagerie

> [!NOTE] Parent Location
> `INPUT[inlineListSuggester(optionQuery(#location),optionQuery(#poi),optionQuery(#Category/PointofInterest)):MyContainer]`

---

## Quest Info

**Type:** `INPUT[inlineSelect(option(main), option(side), option(world), option(rumor), option(personal)):quest_type]`  
**Status:** `INPUT[inlineSelect(option(Rumor), option(Not Started), option(In Progress), option(Complete), option(Failed), option(Abandoned)):questStatus]`  
**Date Obtained:** `INPUT[datePicker:questObtained]`  
**Quest Giver:** `INPUT[suggester(optionQuery(#Category/People), optionQuery(#npc)):questGiver]`  
**Quest Location:** `INPUT[suggester(optionQuery(#location), optionQuery(#poi)):questLocationObtained]`  
**Session Obtained:** `INPUT[suggester(optionQuery(#Category/Journal), optionQuery(#session)):questSessionObtained]`

---

## Operation Goal

Determine whether Marika's Menagerie is merely an extraordinary traveling circus... or something far stranger.

---

## Rumor

> "If Marika's Menagerie ever comes to town...
>
> Go.
>
> Just...
>
> Don't stay too long."

Travelers speak of an impossible circus that appears without warning before quietly disappearing days later.

Its performers include yokai, kitsune acrobats, masked dancers, impossible beasts, and wonders few believe could truly exist.

Some claim it is the greatest spectacle in all of Droshar.

Others refuse to speak of it at all.

---

## Known Details

- The Menagerie appears throughout Droshar but is most often seen in the Southern Principalities.
- Its arrival is never announced.
- Performers come from many races and cultures.
- No two visitors describe Marika the same way.
- The circus is said to disappear as suddenly as it arrives.

---

## Current Leads

- [ ] Discover when the Menagerie next appears.
- [ ] Learn who—or what—Marika truly is.
- [ ] Speak with previous visitors.

---

# Hidden Data

## Truth

Unknown.

Even the Lotus Choir possesses only fragmented reports.

Many operatives have investigated the Menagerie.

Few reached the same conclusions.

---

## Marika Morrow

Believed to be the proprietor of the Menagerie.

Every witness describes Marika differently.

Some insist she is human.

Others swear she is a kitsune, tengu, oni, changeling—or something else entirely.

One detail remains consistent:

Marika always appears to be exactly the person each visitor expects to meet.

Whether this is illusion, transformation, or something stranger remains unknown.

---

## Rumors

Not all stories can be true.

- The Menagerie travels between worlds.
- Time passes differently beneath its tents.
- Every performer joined willingly.
- Nobody has ever successfully followed it.
- Some visitors return fundamentally changed.
- Some return unable to find joy anywhere else.

---

## Potential Rewards

💰 [[Compendium/Rules & Homebrew/Reward Palette (Southern Principalities)#Coin & Valuables\|Festival prizes]]

🧿 [[Compendium/Rules & Homebrew/Reward Palette (Southern Principalities)#Consumables\|Fortune Charm]]

📜 [[Compendium/Rules & Homebrew/Reward Palette (Southern Principalities)#Information (Downtime)\|Performer journals]]

🤝 [[Compendium/Rules & Homebrew/Reward Palette (Southern Principalities)#Favors\|Traveling performer contact]]

✨ [[Compendium/Rules & Homebrew/Reward Palette (Southern Principalities)#Story Rewards\|An invitation to return]]

---

## GM Notes

Treat the Menagerie like folklore.

Every witness should remember something different.

Never explain every mystery.

The uncertainty is part of its charm.

Should the party pursue this rumor, it can naturally expand into a full location, cast of performers, and standalone adventure.

---

> [!column|flex 3]
>> [!important]- PEOPLE
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected People
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/NPC's")
>>         - file.hasLink(this.file)
>> ```
>
>> [!example]- LOCATIONS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected Locations
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Atlas")
>>         - file.hasLink(this.file)
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
>> ```