---
{"dg-publish":true,"dg-path":"2-Lore/Events/Ash War.md","permalink":"/2-lore/events/ash-war/","tags":["event/personal"],"dg-note-properties":{"type":"event","tags":["event/personal"],"aliases":["War of Ash and Dawn"]}}
---


###### Ash War
<span class="sub2">:FasCalendarDays: Personal Event</span>
___

> [!quote|no-t]
> ## The War of Ash and Dawn
> *"In the elder days, the world cracked beneath their steps. The Titans would not yield, and the Gods would not bow. From their clash came fire, storm, and silence — and the world we inherit."*  
> —Fragment of the Dawn Hymn

---

## Name
The conflict between the [[Compendium/Lore/Deities/Titans\|Titans]] and the [[Compendium/Lore/Deities/Gods\|Gods]] is remembered as  **The War of Ash and Dawn**.  
- **Ash:** Symbolizing the ruin left in the wake of the Titans’ fall — mountains shattered, seas boiled, and forests burned to cinder.  
- **Dawn:** Marking the rise of the [[Compendium/Lore/Deities/Gods\|Gods]], who claimed the world from the ashes, shaping order and civilization in place of raw chaos.

---

## Nature of the War
- **The Titans’ Claim:** The [[Compendium/Lore/Deities/Titans\|Titans]] saw the world as their body — every stone and stream their own essence. They raged against the idea of any higher beings seeking to rule or reshape it.  
- **The Gods’ Claim:** The [[Compendium/Lore/Deities/Gods\|Gods]], rising from the void, sought to impose structure, law, and mortal life upon the raw chaos left by titanic creation.  
- **The Struggle:** Neither side could wholly destroy the other. Instead, they tore the world asunder. Mountain ranges split, seas flooded, and the skies filled with firestorms of raw creation energy.  

---

## Outcome
- **The Silence of the Titans:** Broken, buried, and scattered, the [[Compendium/Lore/Deities/Titans\|Titans]] ceased to walk the land. Some believe they died; others say they dream beneath the earth, their breath flowing as [[Compendium/Lore/Objects/Leylines\|leylines]].  
- **The Dominion of the Gods:** Victorious yet diminished, the [[Compendium/Lore/Deities/Gods\|Gods]] withdrew to their celestial realms, leaving mortals to inherit the wounded world.  
- **The Legacy:** Every ley surge, every titan bone, every hymn that shakes the mountains is a scar of the **[[Compendium/Lore/Events/Ash War\|war of ash and dawn]]** — a reminder that neither Titans nor Gods were ever truly defeated.

---

## Cultural Memory
- **Druids:** See it as proof that balance must be preserved, lest the world be torn again.  
- **Scholars:** Treat it as allegory for natural disasters, though leyline surges suggest otherwise.  
- **Priests:** Praise the Gods for their victory, but many secretly fear the Titans’ return.  
- **Giants:** Claim to be the last Children of Ash, tasked with keeping the Titans’ memory alive until they rise again.  



<span class="clearfix"></span>

> [!column|flex 3]
> > [!hint]- NPC's
> > ```base
> > properties:
> >   file.name:
> >     displayName: Name
> > views:
> >   - type: table
> >     name: Name
> >     filters:
> >       and:
> >         - file.inFolder("Compendium/NPC's")
> >         - file.hasLink(this.file)
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