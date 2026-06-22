---
{"dg-publish":true,"dg-path":"1-Droshar/Northern Reaches/Northspires/Northspires.md","permalink":"/1-droshar/northern-reaches/northspires/northspires/","tags":["location/mountain"],"dg-note-properties":{"type":"locale","locations":["[[Northern Reaches]]"],"tags":["location/mountain"]}}
---


![banner.jpg\|banner](/img/user/Assets/Images/banner.jpg)
###### Northspires
<span class="sub2">:FasMountain: Mountain</span>
___

> [!quote|no-t] SUMMARY
># The Northspires
>
> *"Sing, o skald, of the lost children of ice, who gave us our home beneath the waves! Sing, o skald, of the first to descend, and all those who followed! Sing, o skald, in praise of those who embraced the surf!"*  
> —Hymn of the First of the Sea

---

## Overview
The **Northspires** are a jagged mountain ring that juts out into the ocean north of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Emberreach/Emberreach\|Emberreach]]. Their peaks are perpetually cloaked in frost, carved by [[Compendium/Lore/Objects/Leylines\|Leylines]] storms that surge across the high cliffs. Old ruins of the frost giant monasteries dot the ridges, silent reminders of the world before the Great [[Compendium/Lore/Events/Ash War\|Ash War]]. Few dare to tread here — not because of the cold alone, but because the mountains hum with unstable biomantic energy, mutating flora, fauna, and unlucky travelers alike.  

The Northspires stand as a frontier of **untamed magic, monstrous threats, and ancient secrets** — but also hold lures for explorers, hunters, and scholars bold enough to risk the climb.

---

## Lore of the Giants

### The Descent
- The frost giants of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Northspires/Hoytkloster/Hoytkloster\|Hoytkloster]] once dwelled in a monastic city at the crown of the Northspires.  
- During the Great [[Compendium/Lore/Events/Ash War\|Ash War]], the sanctuary was shattered. Giants were cast into the sea.  

---

## Current Dangers
- **[[Compendium/Lore/Objects/Leylines\|Leylines]] Surges:** Wild [[Compendium/Lore/Objects/Biomancy\|biomancy]] warps creatures and terrain unpredictably. Plants gain monstrous sentience, beasts grow twisted.  
- **Undocumented Monsters:** The north spawns horrors seen only in local legends. Hunters tell of creatures that can never be slain the same way twice.  
- **Ruins of [[Compendium/Atlas/Material Plane/Rushthan/Droshar/Northern Reaches/Northspires/Hoytkloster/Hoytkloster\|Hoytkloster]]:** Frost giant relics slumber in ice caves and broken monasteries, tempting treasure-seekers.  

---

## Reasons to Enter the Northspires
- **Ancient Relics:** Frost giant artifacts and lost magics await discovery.  
- **[[Compendium/Lore/Objects/Leylines\|Leylines]] Studies:** Scholars (and reckless biomancers) seek to harness the region’s unstable energy.  
- **Monster Hunts:** Guilds pay handsomely for proof of northern horrors.  
- **Pilgrimage:** Some northern cults claim enlightenment lies in retracing the “path of the Descent.”  

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