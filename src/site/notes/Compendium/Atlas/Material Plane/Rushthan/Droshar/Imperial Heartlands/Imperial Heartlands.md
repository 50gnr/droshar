---
{"dg-publish":true,"dg-path":"1-Droshar/Imperial Heartlands/Imperial Heartlands.md","permalink":"/1-droshar/imperial-heartlands/imperial-heartlands/","tags":["location/generalRegion"],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":["location/generalRegion"],"aliases":["Heartlands","heartlands"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### Imperial Heartlands
<span class="sub2">:FasMap: General Region</span>
___

> [!quote|no-t] SUMMARY
># The  Heartlands
>
> *"Salren is not the Empire. The Heartlands are the Empire. They are its blood, its stone, its chains."*  
> —Frontier proverb

---

## Overview
The **Imperial Heartlands** form the political and cultural core of the Empire, stretching outward from [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Imperial Heartlands/The Capital/Salren/Salren\|Salren]] in fertile plains, well-ordered towns, and ancient trade roads. Unlike the wild frontier of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] or the fractured lands of the Northspires, the Heartlands embody **stability, order, and the dominance of the Dawn Gods**.  

Here, the rule of [[Emperor Kael Vorrath\|Emperor Kael Vorrath]] is uncontested, and loyalty to the Empire is ingrained from birth.

---

## Geography
- **Fertile Plains:** Wide, rolling farmland feeds the cities and legions.  
- **Leyline Stability:** Unlike the North, the Heartlands benefit from the relative calm of the [[Salren Convergence\|Salren Convergence]], making magic predictable and reliable.  
- **Stone Roads:** The old Veynar kings laid great highways of titan-bone and stone, still used by Imperial legions today.  
- **Walled Cities:** Each Heartland city is fortified — less for defense against beasts, more to remind citizens of Imperial authority.  

---

## Culture
- **Faith:** The Dawn temples dominate every town square. Worship of the [[Gods of Dawn\|Gods of Dawn]] is both faith and civic duty.  
- **Law & Order:** Life is heavily regulated; guilds, trade, and even festivals are overseen by Imperial edict.  
- **Pride in Stability:** Citizens see themselves as civilized, contrasting their lives with the “chaotic wilds” of the frontier.  
- **Suspicion of the North:** Hunters and druids are seen as dangerous, half-pagan relics of a world best left behind.  

---

## Politics
- **Centralized Rule:** All governors are appointed directly by Salren. No Heartland city is autonomous.  
- **Military Presence:** Each major settlement maintains a permanent garrison, both to defend and to enforce.  
- **Imperial Spies:** The *Eyes of Kalem* operate openly here, listening for treason or Titan sympathies.  
- **Support for Vorrath:** Most Heartland nobles support the usurper, Kael Vorrath, seeing him as the strong hand they were promised.  

---

## Economy
- **Agriculture:** Grain, vineyards, and livestock sustain both Heartlands and frontier garrisons.  
- **Trade Hub:** Salren’s position at the Bay of Hugger makes the Heartlands the Empire’s commercial engine.  
- **Mining & Crafting:** Titan-bone quarries and ley-stone refineries are exploited under heavy control.  
- **Imperial Coin:** Heartland markets thrive, but always at Imperial tariffs.  

---

## Heartland Cities (Examples)
- **Salren:** The capital and crown of the Empire.  
- **Cindralis:** Known for its vineyards and the Grand Temple of Seraphis.  
- **Duravel:** Military hub, home of the Iron Gate Legion.  
- **Averran:** A trade city on the Bay, where Imperial fleets gather.  

---

## Rumors & Whispers
- *“The Silver Stag Still Runs”*: Sympathizers to the fallen [[House of Veynar\|House of Veynar]] secretly plot rebellion, even in the Heartlands.  
- *“The Convergence Cracks”*: Scholars whisper that the [[Salren Convergence\|Salren Convergence]] is becoming unstable, and Vorrath’s chains may fail.  
- *“The Silent Prison”*: Beneath the Heartlands lies a dungeon where Vorrath keeps something too dangerous to reveal — some say a Titan fragment, others a Veynar heir.  

---




> [!column|flex 3]
> > [!hint]- NPC's
> > ```base
> > formulas:
> >   LinkedIndirectly: |
> >     locations.contains(this.file)
> >     || list(locations)
> >          .filter(file(value)
> >            && list(file(value).properties.locations).contains(this))
> >          .length > 0
> > 
> > properties:
> >   file.name:
> >     displayName: Name
> > 
> > views:
> >   - type: table
> >     name: This Location Only
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - locations.contains(this.file)
> > 
> >   - type: table
> >     name: Sub-Locations Included
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - formula.LinkedIndirectly
> > ```
>
>> [!example]- LOCATIONS
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Provinces
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/Atlas")
> >         - locations.contains(this.file)
> > ```
>
>> [!note]- HISTORY
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Session Notes
> >     filters:
> >       and:
> >         - file.inFolder("Session Notes")
> >         - file.hasLink(this.file)
> > ```