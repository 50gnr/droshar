---
{"dg-publish":true,"dg-path":"2-Lore/Rumors/Gung & Sung.md","permalink":"/2-lore/rumors/gung-and-sung/","tags":["Category/Quest","quest","personal","downtime","temporal-anomaly"],"dg-note-properties":{"type":"quest","tags":["Category/Quest","quest","personal","downtime","temporal-anomaly"],"MyContainer":["[[Sung and Gung\|Sung and Gung]]"],"MyCategory":null,"quest_type":"personal","questObtained":null,"questStatus":"Rumor","questGiver":null,"questLocationObtained":"[[Sung and Gung\|Sung and Gung]]","questSessionObtained":null,"questNotes":null,"questLootAvail":null,"questLookEarned":null,"cover":"[[Sung and Gung.png]]","obsidianUIMode":"preview"}}
---


## Summary

During a quiet evening at [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/In'nali/Sung & Gung\|Sung & Gung]], [[Compendium/Party/Player Characters/Maeva the Chosen\|Maeva]] and [[Compendium/Party/Player Characters/ShoSlovak Trogaro\|Sho]] discover that the basement's reigning chicken-combat champion has somehow become two identical birds.

Both possess the same scars.

Both recognize their handler.

Both appear convinced they won last night's match.

---
# Hidden Data
## Objectives

- [ ] Determine which chicken belongs in the current timeline.
- [ ] Learn what caused the duplication.
- [ ] Resolve the anomaly without disrupting the evening's matches.
- [ ] Keep the incident from becoming a public spectacle.

---

## Known Details

- The duplication occurred sometime after the basement closed.
- Neither bird behaves like an illusion.
- Both remember events that only one chicken should have experienced.
- A cracked drinking cup nearby briefly repairs itself whenever Sho approaches.
- Maeva recognizes the sensation from the first anomaly she and Sho sealed together.

---

## Important NPCs

- [[Lady Maeva the Chosen\|Lady Maeva the Chosen]]
- [[Compendium/Party/Player Characters/ShoSlovak Trogaro\|ShoSlovak Trogaro]]
- Proprietors of [[Sung and Gung\|Sung and Gung]]
- The chicken's increasingly distressed handler

---

## Important Locations

- [[Sung and Gung\|Sung and Gung]]
- The basement chicken-combat ring
- The locked storage room beneath the stairs

---

## Current Leads

- [ ] Compare the chickens' memories and behaviour.
- [ ] Examine the basement for temporal disturbances.
- [ ] Question anyone present after closing.
- [ ] Decide whether one bird must be removed—or whether both now belong.

---

## Resolution

A tiny temporal fracture has formed around an old wager token wedged beneath the fighting ring.

The token was present during one of Sho and Maeva's earliest nights at Sung & Gung. Their combined presence has awakened a harmless echo of two possible outcomes:

- In one timeline, the champion won.
- In the other, it lost and was replaced.

Both chickens are real.

Removing or sealing the wager token collapses the fracture, but Sho and Maeva must decide which outcome remains.

A sufficiently strong result may allow them to stabilize both birds without damaging the timeline.

---

## Encounter

### Exploration / Social

The encounter should revolve around:

- identifying temporal inconsistencies
- questioning regular patrons
- managing the handler's growing panic
- keeping the basement crowd entertained and unaware
- deciding what constitutes the “correct” outcome

The better the rolls, the cleaner the resolution.

Poor results create increasingly visible anomalies:

- repeated conversations
- drinks refilling themselves
- wagers changing after being placed
- a match beginning twice
- patrons briefly remembering different winners

---

## Rewards / Loot

**Available:** `INPUT[suggester(optionQuery(#item)):questLootAvail]`  
**Earned:** `INPUT[suggester(optionQuery(#item)):questLookEarned]`

🤝 [[Prep/Southern Prince C2/Reward Palette (Southern Principalities)#Favors\|Free drinks and basement access]]

📜 [[Prep/Southern Prince C2/Reward Palette (Southern Principalities)#Information (Downtime)\|A clearer understanding of their shared temporal signature]]

✨ [[Prep/Southern Prince C2/Reward Palette (Southern Principalities)#Story Rewards\|A private tradition shared by Sho and Maeva]]

---

## GM Notes

Keep this light.

The anomaly is strange, inconvenient, and personal—but not immediately dangerous.

The real purpose is to:

- establish [[Sung and Gung\|Sung and Gung]] as Sho and Maeva's shared place
- show how comfortable they are working together
- revisit their temporal history without exposing everything
- give them a complete downtime story in one sitting

---

## Truth

The fracture is not evidence that the original anomaly has reopened.

It does, however, suggest that Sho and Maeva continue to disturb time when they remain together in emotionally significant places.

Whether this is harmless resonance or a warning remains undecided.

---

## Complications

- A regular wants to buy the duplicate chicken.
- The handler refuses to accept that either bird is expendable.
- One chicken appears terrified of Sho.
- The other follows Maeva everywhere.
- A patron remembers Maeva wearing a face she has never used.
- Sung or Gung has seen this happen before and refuses to elaborate.

---

## Future Development

This quest may later point toward:

- the original sealed anomaly
- recurring temporal echoes around Sho and Maeva
- an outside force tracking paradox activity
- evidence that their arrival in this timeline was not accidental

None of these developments need to be decided during the downtime session.

---

> [!column|flex 3]
>> [!hint]- PEOPLE
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