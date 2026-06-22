---
{"dg-publish":true,"permalink":"/compendium/atlas/material-plane/rushthan/droshar/northern-reaches/crownkeep-mountains/crownkeep-mountains/","tags":["location/mountain"],"dg-note-properties":{"type":"locale","locations":["[[Northern Reaches]]","[[The Capital]]"],"tags":["location/mountain"],"aliases":["The Coilspines","The Coilspine","The Crownkeep","Crownkeep","Coilspine"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### Crownkeep Mountains
<span class="sub2">:FasMountain: Mountain</span>
___

> [!quote|no-t] SUMMARY
> ## The Coilspine / Crownkeep Mountains
> *"To the Empire, it is a crown upon their brow. To us, it is the bones of a serpent yet to wake."*  
> —Derric Harthorne, Hearthfire Hall

---

## Overview
Stretching from **Greenshire** in the west to **Drassig** in the east, this massive mountain range dominates southern Droshar. Its jagged peaks rise like fangs through the clouds, their ridges curling and twisting as though coiled in sleep. Deep within its heart lies the dormant volcano that forms **Veythar’s Maw**, the so-called *Never-Ending Dungeon*.  

The range is known by two names:  

- **The Crownkeep Mountains** (Imperial Name): Celebrated in Salren as a symbol of divine dominion, a “crown” upon the Empire’s brow. Imperial cartographers mark it with grandeur, ignoring its dangers.  
- **The Coilspine** (Local Name): To hunters, druids, and frontier folk, the range is the petrified remains of **Veythar, the Verdant Coil**, a titan whose body still twists beneath the land. Earthquakes, avalanches, and leyline storms are said to be his restless stirring.  

---

## Features
- **[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Crownkeep Mountains/Veythar's Maw/Veythar's Maw\|Veythar's Maw]]:** The dormant volcano and labyrinthine cave hidden in the southern forest.  
- **Twisting Peaks:** The ridgelines curl unnaturally, resembling bones or scales turned to stone.  
- **[[Compendium/Lore/Objects/Leylines\|Leyline]] Surge Zones:** Frequent magical storms ripple along the range, reshaping flora and fauna.  
- **Lost Passes:** Trails through the Coilspine shift after quakes; some lead to forgotten ruins, others to sudden death.  

---

## Cultural Views
- **Imperial Propaganda:** Priests of the Dawn Gods claim the Crownkeep was raised when [[Auramar\|Auramar]] struck down a titan, sealing its chaos beneath divine law.  
- **Frontier Belief:** Druids insist the [[titan\|titan]] still sleeps below — its awakening would tear the land apart.  
- **Hunter’s Tales:** Old [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]] stories warn that “each fang that breaks the sky is a bone in the beast yet to rise.”  

---

## Rumors
- **The Burning Crown:** When the Maw trembles, red light flickers on the mountain crests, as though the peaks wear a crown of fire.  
- **The Hollow Coil:** Some miners claim to have broken into caverns shaped like ribcages far below. They fled when the walls began to *breathe.*  
- **The Emperor’s Secret:** A forbidden legend says the Emperor seeks to carve a throne from the Maw itself, to sit where a Titan’s heart once beat.  


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
> >     name: Landmarks
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