---
{"dg-publish":true,"dg-path":"2-Lore/Rumors/Stillwater Array.md","permalink":"/2-lore/rumors/stillwater-array/","tags":["Category/Quest","quest","quest/active"],"dg-note-properties":{"type":"quest","tags":["Category/Quest","quest","quest/active"],"quest_type":"main","questStatus":"Active","questGiver":"[[Compendium/NPC's/Southern Principalities/Shōren Vale|The Quiet Fox]]","questLocationObtained":"[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Shigure Compound]]","questSessionObtained":"[[Session Notes/C2 Southern Principalities/Session 09 - Find the Thread]]","locations":["[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Shigure Compound]]","[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Southern Principalities/Bardune/Bardune]]"],"cover":"[[Assets/Images/SP-Scene/Shigure/Shigure Steps.png]]","obsidianUIMode":"preview"}}
---


# Stillwater Array

## Operation Goal

Research the three separated elements of Bardune's Stillwater Array, choose one, and use its movement to discover where the complete Array will be assembled.

## Mission Brief

> During the Hakuryū crisis, Bardune constructed a means of containing what could not be calmed.
>
> It is called the **Stillwater Array**.
>
> Its three elements remain separated:
>
> - a spiritual vessel held beyond Bardune
> - four ritual anchors concealed within the city
> - an activating bell kept above it
>
> Bardune will bring them together for the Array's first complete assembly.
>
> Research the three elements and their custodians.
>
> Choose one.
>
> Learn the location or follow it to the convergence site.
>
> Do not prevent its delivery. Do not reveal that the Array is known.
>
> Otherwise, the use of force is authorized at your discretion.
>
> Once the convergence site is confirmed, further instructions will follow.

## Active Objectives

- [ ] Research the **Heart**, its custodian, and its movement
- [ ] Research the **Anchors**, their custodian, and their movement
- [ ] Research the **Bell**, its custodian, and its movement
- [ ] Establish the shared transport window
- [ ] Choose one component to pursue
- [ ] Prepare an initial approach
- [ ] Follow the selected component without preventing its delivery
- [ ] Identify the convergence site

## Starting Leads

### Heart

> “Bardune entrusted the vessel to a people who can disappear beneath the southern sea.”

### Anchors

> “Four living stakes sleep beneath a garden that never closes.”

### Bell

> “The final word waits where the city's rivers look like silver thread.”

## Operational Limits

- Do not reveal that the Stillwater Array is known.
- Do not prevent the chosen component from reaching the convergence.
- Further instructions will follow once the convergence site is confirmed.

## Assigned Operatives

- [[Compendium/Party/Player Characters/Player Facing/Maeva\|Maeva]]
- [[Compendium/Party/Player Characters/Player Facing/Clay\|Clay]]
- [[Compendium/Party/Player Characters/Player Facing/Nobu\|Nobu]]
- [[Compendium/Party/Player Characters/Player Facing/Sho\|Sho]]
- [[Compendium/Party/Player Characters/Player Facing/Maki\|Maki]]

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
