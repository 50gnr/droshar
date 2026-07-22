---
{"dg-publish":true,"dg-path":"2-Lore/Rumors/The Four Shrines.md","permalink":"/2-lore/rumors/the-four-shrines/","tags":["Category/Quest","quest"],"dg-note-properties":{"type":"quest","tags":["Category/Quest","quest"],"MyContainer":["[[The Four Shrines|The Four Shrines]]"],"MyCategory":null,"quest_type":"main","questObtained":null,"questStatus":"Not Started","questGiver":"[[Compendium/NPC's/Southern Principalities/Shōren Vale\|The Quiet Fox]]","questLocationObtained":"[[Shigure Compound]]","questSessionObtained":"[[Session 1 - The Quiet Fox Calls]]","questNotes":null,"questLootAvail":["12,000gp","5-8 Consumables","2r 1vr meaningful items"],"questLookEarned":null,"cover":"[[hakuryu valley regional.png]]","obsidianUIMode":"preview"}}
---


# Four Bakuryō Shrines


## Operation Goal

Recover the Four Offerings from the Bakuryō Shrines without drawing unnecessary attention.

---

## Mission Brief

> Operatives,
>
> Four shrines within the Hakuryū Valley have been selected for investigation.
>
> Recover all offerings presently maintained within these sites.
>
> Avoid unnecessary attention.
>
> Preserve operational secrecy.
>
> Further intelligence has been prepared within the Shigure Archive.
>
> — [[Compendium/NPC's/Southern Principalities/Shōren Vale\|The Quiet Fox]]

---

## Objectives

- [ ] Recover the offering from the [[Prep/Southern Prince C2/Arc 1#Location - Farm\|Farmer's Shrine]]
- [ ] Recover the offering from the [[Prep/Southern Prince C2/Arc 1#Location - Rapids\|Shrine of the Rapids]]
- [ ] Recover the offering from the [[Prep/Southern Prince C2/Arc 1#Location - Mirror Lake\|Mirror Lake Shrine]]
- [ ] Recover the offering from the [[Prep/Southern Prince C2/Arc 1#Location - Falling Clouds\|Monastery of Falling Clouds]]
- [ ] Return all recovered offerings to [[Compendium/NPC's/Southern Principalities/Shōren Vale\|The Quiet Fox]]

---

## Known Details

The Shigure Archive records indicate:

- Four Bakuryō Shrines remain active throughout Hakuryū Valley.
- Each shrine safeguards a ceremonial offering.
- The shrines continue to serve nearby communities.
- Operational secrecy is expected at all times.
- No explanation has been provided for why these particular shrines were selected.

---

## Important NPCs

- [[Compendium/NPC's/Southern Principalities/Shōren Vale\|The Quiet Fox]]
- Shrine Caretakers (Unknown)

---

## Important Locations

- [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Hakuryū Valley\|Hakuryū Valley]]
- [[Prep/Southern Prince C2/Arc 1#Location - Farm\|Farmer's Shrine]]
- [[Prep/Southern Prince C2/Arc 1#Location - Rapids\|Shrine of the Rapids]]
- [[Prep/Southern Prince C2/Arc 1#Location - Mirror Lake\|Mirror Lake Shrine]]
- [[Prep/Southern Prince C2/Arc 1#Location - Falling Clouds\|Monastery of Falling Clouds]]

---

## Current Leads

- [ ] Study the Shigure Archive.
- [ ] Decide the shrine visitation order.
- [ ] Prepare cover identities.
- [ ] Gather equipment and supplies.
- [ ] Develop an operational plan.

---

# Hidden Data

## Truth

The offerings are not merely ceremonial relics.

Together they anchor an ancient Bakuryō ritual that quietly maintains the natural flow of the Hakuryū River.

Removing all four offerings completes the first phase of Hoshi Reedmark's plan.

The party believes they are completing a routine retrieval mission.

They are unknowingly dismantling the valley's oldest safeguard.

---

## Bakuryō's Purpose

Each shrine protects one of Bakuryō's Four Offerings.

Removing a single offering causes little immediate concern.

Only when the fourth offering is taken does the ritual finally collapse.

The Hakuryū River reverses.

Bakuryō awakens.

---

## Story Progression

### Shrine One

A simple retrieval.

The mission appears routine.

---

### Shrine Two

Caretakers begin noticing missing offerings.

Local rumors slowly spread.

---

### Shrine Three

Wardens increase patrols.

Travel throughout the valley becomes more scrutinized.

---

### Shrine Four

The final offering is removed.

The Hakuryū River reverses.

Arc I concludes.

Arc II begins.

---

## Complications

Possible complications include:

- Curious villagers
- Shrine festivals
- Unexpected visitors
- Weather
- Wandering pilgrims
- Warden patrols
- Shrine caretakers
- Yokai encounters
- Local wildlife

---

## Rewards / Loot

**Available:** `INPUT[suggester(optionQuery(#item)):questLootAvail]`  
**Earned:** `INPUT[suggester(optionQuery(#item)):questLookEarned]`

### Immediate

- Lotus Choir payment
- Increased trust within the Choir

### Long Term

- Completion of Arc I
- Story progression
- Reputation
- Future opportunities

---

## GM Notes

The shrines should never feel like dungeons.

Each should feel like a living place maintained by ordinary people fulfilling ordinary duties.

The players should never suspect the true purpose of the offerings until after the fourth shrine.

---

## Future Development

Upon completion:

- The Hakuryū River reverses.
- Public panic begins.
- Bakuryō stirs.
- Hoshi Reedmark advances to Phase Two.
- The Lotus Choir begins to question the mission.

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