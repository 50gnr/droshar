---
{"dg-publish":true,"dg-path":"1-Droshar/Southern Principalities/Southern Principalities.md","permalink":"/1-droshar/southern-principalities/southern-principalities/","tags":["location/generalRegion"],"dg-note-properties":{"type":"territory","locations":["[[Droshar]]"],"tags":["location/generalRegion"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
# The Southern Principalities
<span class="sub2">:FasMap: General Region</span>
___

> [!quote|no-t] SUMMARY
>  _“The South endures not because it is strong—but because it is dangerous to rule.”_


- **Centers:** Bardune, In’nalii
    
- **Identity:**  
    A chain of ancient principalities nestled among bamboo valleys, mist-choked mountains, and fractured coastlines. These lands predate the Empire and were never fully conquered—only _contained_. Power here is local, ritualized, and deeply entangled with place. Authority flows through oaths, bloodlines, monasteries, and traditions whose original purposes are half-forgotten.
    
- **Tone:**  
    Mythic, restrained, and quietly dangerous.  
    The South does not posture; it _waits_. Beauty masks dread. Honor exists, but it is older and heavier than chivalry—measured in generations, not duels. When violence erupts, it is sudden, catastrophic, and never clean.
    
- **Cultural Markers:**  
    Bamboo architecture, mountain shrines, coastal watch-temples, and artisan traditions shaped by scarcity and restraint. Stories of “sleeping gods,” mountain spirits, and sea-borne colossi are common—but spoken of as warnings, not legends.
    
- **Political Reality:**  
    Nominally Imperial territory, but functionally autonomous. Imperial law is enforced selectively and often at a distance. Direct military occupation is rare and historically short-lived. The Empire governs here through treaties, proxies, and careful ignorance.
    
- **Key Role:**  
    A pressure point in the Empire’s stability.  
    The Southern Principalities do not rebel because rebellion would wake things best left undisturbed. Secession is always _possible_, never _threatened_, and understood by all parties to be catastrophic if mishandled.
    

---
# The Road Between Bardune and In'nali (or lack thereof)

Despite their proximity, **there is no direct road**.

- The forest-lake terrain and cliff-faces make straight routes taboo
    
- Ancient treaties forbid cutting certain valleys or passes
    
- All trade routes loop _north or south_, adding weeks of travel
    

This is not inefficiency.  
It is **containment**.

Both cities quietly agree that **some spaces must remain untraveled**.

---

# Sets of Tensions (Yokai-Appropriate, Non-Combat)

These are not “good vs evil.”  
They are **irreconcilable truths**.

---

## 1. **Appeasement vs Containment**

- **Bardune:** Spirits must be soothed, remembered, and honored
    
- **In’nali:** Spirits must be sealed, watched, and prepared for
    

Neither side denies the danger—only _how_ to live with it.

This creates:

- Disputes over shrine practices
    
- Conflicting responses to omens
    
- Passive resistance instead of confrontation
    

---

## 2. **Memory vs Readiness**

- **Bardune:** The past teaches restraint
    
- **In’nali:** The past teaches preparation
    

Bardune records _what happened_.  
In’nali plans for _what might happen again_.

This affects:

- How kaiju legends are preserved
    
- Whether old rituals are repeated or retired
    
- What knowledge is shared with outsiders
    

---

## 3. **Silence vs Signal**

- **Bardune:** Silence keeps sleepers dormant
    
- **In’nali:** Signals are required to monitor threats
    

Wind-horns, beacon-fires, seismic wards—In’nali uses them all.  
Bardune believes each is a **provocation**.

Neither can prove they’re right.

---

## 4. **Trade as Exchange vs Trade as Risk**

- **Bardune:** Trade spreads stories, softens borders
    
- **In’nali:** Trade spreads weaknesses
    

So:

- Bardune favors open markets and mixed caravans
    
- In’nali insists on inspections, seals, and escort rites
    

No tariffs.  
Just _friction_.

---

## 5. **Who Should Wake the Sleeper (If Anyone Ever Does)**

This is the unspoken core.

- Bardune believes **no one has the right**
    
- In’nali believes **someone must be prepared to**
    
---
They have never said this aloud in the same room.


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