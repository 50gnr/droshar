---
{"dg-publish":true,"permalink":"/compendium/lore/calendar/","tags":["event/seasonal"],"dg-note-properties":{"type":"event","tags":["event/seasonal"]}}
---


# Calendar


## 📜 The Reckoning of Ash 

> **The Reckoning of Ash (RA)**  
> _“Counted from the silence that followed the last titanfall.”_
    

The Empire uses it officially.  
The Lodge uses it **loosely**.  
The Amethyst Moon rejects it entirely.

---


### **0 RA — The Ash Silence**

- The War of Ash and Dawn ends.
    
- Titans fall, shatter, or sleep.
    
- Gods withdraw.
    
- Leylines stabilize _temporarily_.
    
- No empire yet — only survivors.
    

---

### **~2400 RA — Founding of Emberreach**

- Frontier hunters settle near exposed Titan Bones.
    
- The Ash Pyre is established early, possibly **before** the Lodge formalizes.
    
- Emberreach predates the current Empire’s authority.
    

> Emberreach is **old enough to have secrets**, but young enough to still bleed.

---

### **~2610 RA — The Usurpation**

- Emperor **Kael Vorrath** seizes the southern throne.
    
- The House of Veynar is destroyed.
    
- A rumored heir vanishes northward.
    
- The Empire shifts from negotiated rule to divine absolutism.
    

This date is **heavily propagandized** in Imperial records.

---

### **~2625–2635 RA — The Violet Spread**

- Biomancy experiments increase.
    
- Leyline storms grow less predictable.
    
- Mutations become harder to hide.
    
- Groups like the **Amethyst Moon** emerge from fringe philosophy into action.
    

Hunters start using words like _“changed”_ instead of _“cursed.”_

---

### **Now: 2637 RA — The Waning Crown**

_(This is the current year.)_

- Imperial reach is strong but strained.
    
- The North is unstable.
    
- The Lodge feels pressure from all sides.
    
- Apprentices face graduation amid growing uncertainty.
    

NPCs might say:

- “The Crown is waning — you can feel it.”
    
- “Storms haven’t been right since thirty-three.”
    
- “This isn’t how hunts were in my father’s day.”

---
# The Droshar Calendar

The modern calendar consists of **11 months of 30 days**, for a total of **330 days per year**.

Years are recorded as **PAW (Post Ash War)**.

---

## Horisal
### The Long Silence

The first month of the year. A time of endurance, reflection, and recovery after the hardships of the previous cycle.

**Greenmark (5th Horisal)** — Doorways are marked with green paint, moss, or evergreen branches to invite renewal.

---

## Misuthar
### The Turning Sky

Winds shift, migrations begin, and communities prepare for the coming season of activity.

**Hunt's Dawn (20th Misuthar)** — Young hunters undertake their first sanctioned hunts.

**20 Misuthar** → Day/night equal (start of the active half of the year)

---

## Dualahei
### First Renewal

Trade routes reopen, roads are repaired, and communities begin new projects and ventures.

**Ember Games (15th Dualahei)** — Competitions of strength, skill, and endurance celebrate survival and renewal.

---

## Thunsheer
### Rising Light

Travel increases, trade flourishes, and ambitions are pursued beneath the year's longest days.

**White Stag Vigil (Final Week)** — Watchers gather in hopes of witnessing the legendary White Stag.

---

## Unndilar
### High Growth

Traditionally associated with abundance, prosperity, and the rewards of hard work.

**Hunt's Feast (20th Unndilar)** — Hunters, storytellers, and communities gather to celebrate the season's successes.

**15 Unndilar** → Longest day of the year.

---

## Brussendar
### The First Fading

Attention shifts from expansion toward preservation as the year begins its gradual decline.

**Emberfall Rite (30th Brussendar)** — Broken tools and charms are ceremonially burned or surrendered.

---

## Sydenstar
### The Gathering Dark

A month of remembrance, tradition, and preparing for the challenges ahead.

**Ashen Vigil (15th Sydenstar)** — Communities honor the memory of those who have passed.

---

## Fessuran
### The Quiet Road

Travel slows and patience is valued. Dreams, omens, and personal reflection hold special significance.

---

## Quen'pillar
### The Lean Moon

Historically associated with sacrifice, restraint, and communal support during difficult times.

---

## Cuersaar
### The Deep Watch

A month devoted to vigilance, preparedness, and guarding against threats both known and forgotten.

---

## Duscar 
### Longnight

The final month of the year, dedicated to endings, remembrance, and enduring together through darkness.

**Longnight Feast (10th Duscar)** — Families and communities gather to share food, warmth, and stories.

**15th Duscar** — Longest Night.
    

   

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