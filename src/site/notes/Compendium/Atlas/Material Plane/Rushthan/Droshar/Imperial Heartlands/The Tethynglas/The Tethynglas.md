---
{"dg-publish":true,"dg-path":"1-Droshar/Imperial Heartlands/The Tethynglas/The Tethynglas.md","permalink":"/1-droshar/imperial-heartlands/the-tethynglas/the-tethynglas/","tags":["location/forest"],"dg-note-properties":{"type":"locale","locations":["[[Imperial Heartlands]]","[[Northern Reaches]]"],"tags":["location/forest"],"aliases":["The Withering Wood","Withering wood","Tethynglas"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/default/banner.jpg)
###### The Tethynglas
<span class="sub2">:FasTree: Forest</span>
___

> [!quote|no-t] SUMMARY
># (The Withering Wood)
> *"The road is shorter through the green, aye. But no road is worth the soul it steals."*  
> —Old Steelholde saying

---

## Overview
Between **[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]** and the Imperial capital of **[[Compendium/Atlas/Material Plane/Rushthan/Droshar/Imperial Heartlands/The Capital/Salren/Salren\|Salren]]** lies the vast, brooding forest of **Tethynglas** (*“the Fading Green”* in old tongue). Its canopy stretches thick as a stormcloud, blotting out the sun and swallowing whole paths. Though it offers the most direct route south, travelers avoid it entirely, skirting wide through [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Blord/Blord\|Blord]] and the [[Esmelan Marches\|Esmelan Marches]] instead.  

The Empire marks it on maps as the **Withering Wood**, though many whisper older names: *The Green Silence, The Veil, The Soulwood.*  

---

## Name & Etymology
- **Tethyn:** “To fade, wither, or pass away” in ancient Giant-Celtic.  
- **Glas:** “Green, pale, or spirit.”  
- Together: *“The Fading Green”* — a forest caught between life and death.  

---

## Features
- **Eternal Canopy:** Little sunlight pierces its roof. The deeper one travels, the more twilight grips the wood.  
- **Shifting Paths:** Roads vanish overnight. Hunters swear the trees themselves move.  
- **Whispering Winds:** Voices ride the breezes. Sometimes they call by name. Sometimes they sing hymns best left forgotten.  
- **[[Compendium/Lore/Objects/Leylines\|Leyline]] Fractures:** Tethynglas is riddled with leyline scars, making it a hotbed of [[Compendium/Lore/Objects/Biomancy\|biomantic]] horrors.  

---

## Rumors & Tales
- **[[Compendium/Lore/Organizations/The Dusk Court\|The Dusk Court]]:** Locals whisper of an ancient fae court that still hunts within the wood, feeding on mortal wanderers. Their revels sound like music, but those who follow never return.  
- **The Titan’s Root:** Some druids believe the forest grew from a root of **[[Compendium/Lore/Deities/Titans\|Veythar, the Verdant Coil]]**, spreading endlessly underground. His corruption still warps its trees.  
- **The [[Compendium/Lore/Creatures/White Stag\|White Stag]]’s Crossing:** Sightings of the White Stag are common here, often leading hunters deeper until they vanish entirely.  
- **The Sleeping Choir:** Imperial scouts claim to have found stone shapes resembling giant throats, as though voices once sang from the earth itself. They fled when one exhaled mist.  
- **The Hollow Men:** Bandits who enter Tethynglas never emerge whole. Some return pale and empty-eyed, their voices hollow echoes of themselves.  
- **The Silent Year:** Once, an entire village disappeared after taking the forest road. A year later, its people stumbled back out — unchanged, except none remembered their names.  
- **The Emperor’s Edict:** It is said the Emperor himself forbade building roads through Tethynglas, calling it a “sealed wound.” No official explanation has ever been given.  

---

## Cultural Views
- **Hunters:** “You don’t hunt in Tethynglas — you’re hunted.”  
- **Druids:** Claim the forest is sacred, a place where the boundary between world and ley is paper-thin.  
- **Imperials:** Fear it as cursed, yet covet the relics and secrets buried within.  
- **Common Folk:** Simply avoid it — and pity the fool who thinks themselves brave.  



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