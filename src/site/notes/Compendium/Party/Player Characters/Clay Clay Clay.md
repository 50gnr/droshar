---
{"dg-publish":true,"dg-path":"4-Party/Clay Clay Clay.md","permalink":"/4-party/clay-clay-clay/","tags":["Category/Player"],"dg-note-properties":{"aliases":["Clay"],"tags":["Category/Player"],"Player":"Wyatt","Role":"Player","level":10,"hp":50,"max_hp":71,"ac":80,"modifier":2,"pasperc":13,"Status":"Active","PlayerKnownLanguages":["Celestial","Common","Dwarvish"],"faction_standing":{"Faction Name 1":1,"Faction Name 3":3},"char_name":"Clay","char_race":"Hanimori","char_class":"Rogue / Barbarian","char_subclass":null,"char_gender":"Male","char_status":"Alive","char_age":"Old AF","char_items":["[[Locate the Eye Ball|Locate the Eye Ball]]","[[z_Templates/World Builder Templates/Template-Quest.md|Template-Quest]]"],"char_image":["[[Clay.png]]"],"Connected_Quests":[],"Connected_Groups":["[[The Lotus Choir]]"],"parents":["Father","Mother"],"partner":["Partner"],"children":["Child"],"enemies":["Enemy"],"allies":["Friend"],"siblings":["Brother","Sister"],"obsidianUIMode":"preview","MyContainer":null,"MyCategory":null}}
---

# Clay

> [!infobox|no-t right]
> ![Assets/Images/Party/Clay.png\|Clay.png](/img/user/Assets/Images/Party/Clay.png)
> ###### Details:
> | Type | Stat |
> | ---- | ---- |
> | :FasCrown: Level   | 10 |
> | :RiSwordFill: Class |  Rogue / Barbarian|
> | :FasUserShield: Archetype |  `=this.char_subclass`|
> |  :FasUserGroup: Race |  Hanimori|
> | :FasArrowsUpDownLeftRight: HP | 50


```badges
items:
  - label: Spell Save
    value: 14
  - label: AC
    value: '{{frontmatter.ac}}'
  - label: AC (Mage Armor)
    value: 15
```
> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🤹Abilities+Skills),
> option(2, ⚔️Inventory),
> option(3, 🔗Connections),
> option(4, 🧑‍🤝‍🧑Relationships),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box-maxh]
> > >[!div-m|no-title]
> > > ![[Compendium/Party/Player Characters/Clay Clay Clay#Skills\|no-h clean]]
> >
> > > ![[Compendium/Party/Player Characters/Clay Clay Clay#Inventory\|no-h1 clean]]
> >
> > > [!div-m|no-title]
> > > ![[Compendium/Party/Player Characters/Clay Clay Clay#Connections\|no-h1 clean]]
> > 
> > > [!div-m|no-title]
> > > ![[Compendium/Party/Player Characters/Clay Clay Clay#Relationships\|no-h1 clean]]

---

# Description

This is the persons description. 

# GM Notes

Make notes of what you need to track in the town here. 



# Hidden Data

# Skills

```ability
abilities:
  strength: 10
  dexterity: 10
  constitution: 10
  intelligence: 10
  wisdom: 10
  charisma: 10

proficiencies:
  - intelligence
  - wisdom
```

<br>

```skills
proficiencies:
  - arcana
  - deception
  - history
  - insight
  - investigation
```

# Inventory

The following items belong to Clay Clay Clay.

Items: `INPUT[inlineListSuggester(optionQuery(#Category/Quest)):char_items]`

#### Ring of Investigation

```consumable
label: ""
state_key: din_items__ring_of_investigation
uses: 3
```

_May the ability to see also provide you with a clear vision. Grants +1 to Investigation rolls._

# Connections

Is the person linked to any groups or quests?

Quests: `INPUT[inlineListSuggester(optionQuery(#Category/Quest)):Connected_Quests]`

Groups: `INPUT[inlineListSuggester(optionQuery(#Category/Group)):Connected_Groups]`

# Relationships

List important relationships here.

<pre class="dataview dataview-error">Evaluation Error: SyntaxError: Invalid or unexpected token
    at DataviewInlineApi.eval (plugin:dataview:19027:21)
    at evalInContext (plugin:dataview:19028:7)
    at asyncEvalInContext (plugin:dataview:19038:32)
    at DataviewJSRenderer.render (plugin:dataview:19064:19)
    at DataviewJSRenderer.onload (plugin:dataview:18606:14)
    at DataviewJSRenderer.load (app://obsidian.md/app.js:1:700894)
    at DataviewApi.executeJs (plugin:dataview:19607:18)
    at DataviewCompiler.eval (plugin:digitalgarden:12473:23)
    at Generator.next (&lt;anonymous&gt;)
    at eval (plugin:digitalgarden:90:61)</pre>mermaid\nflowchart LR\n" +
  (parents.length > 0 ? parents.map((parent, index) => `P${index + 1}[${parent}]:::internal-link\nP${index + 1} --> Current\n`).join('') : '') +
  `Current[${current}]\n` +
  (partner.length > 0 ? `PT[Partner]\nCurrent --> PT\n` : '') +
  (partner.length > 0 ? partner.map((p, index) => `PT${index + 1}[${p}]:::internal-link\nPT --> PT${index + 1}\n`).join('') : '') +
  (children.length > 0 ? `C[Children]\nCurrent --> C\n${children.map((child, index) => `C${index + 1}[${child}]:::internal-link\nC --> C${index + 1}\n`).join('')}` : '') +
  (siblings.length > 0 ? `S[Siblings]\nCurrent --> S\n${siblings.map((sibling, index) => `S${index + 1}[${sibling}]:::internal-link\nS --> S${index + 1}\n`).join('')}` : '') +
  (enemies.length > 0 ? `E[Enemies]\nCurrent --> E\n${enemies.map((enemy, index) => `E${index + 1}[${enemy}]:::internal-link\nE --> E${index + 1}\n`).join('')}` : '') +
  (allies.length > 0 ? `A[Allies]\nCurrent --> A\n${allies.map((ally, index) => `A${index + 1}[${ally}]:::internal-link\nA --> A${index + 1}\n`).join('')}` : '') +
  `class ${parents.length > 0 ? parents.map((_, index) => `P${index + 1},`).join('') : ''}Current${children.length > 0 ? children.map((_, index) => `C${index + 1},`).join('') : ''}${siblings.length > 0 ? siblings.map((_, index) => `S${index + 1},`).join('') : ''}${enemies.length > 0 ? enemies.map((_, index) => `E${index + 1},`).join('') : ''}${allies.length > 0 ? allies.map((_, index) => `A${index + 1},`).join('') : ''} internal-link;`
)
```

> [!NOTE]- Relationship Config - Enter name of People Notes
> `BUTTON[button_person]` Nodes will link to notes of the same name.
>
> | Parents | Partner | Children |
> | --- | --- | --- |
> | `INPUT[list:parents]` | `INPUT[list:partner]` | `INPUT[list:children]` |
>
> | Siblings | Enemies | Allies |
> | --- | --- | --- |
> | `INPUT[list:siblings]` | `INPUT[list:enemies]` | `INPUT[list:allies]` |

# Faction Standing

<div><table class="dataview table-view-table"><thead class="table-view-thead"><tr class="table-view-tr-header"><th class="table-view-th"><span>Faction</span></th><th class="table-view-th"><span>Your Standing</span></th><th class="table-view-th"><span>Benefits</span></th><th class="table-view-th"><span>Primary Contact</span></th></tr></thead><tbody class="table-view-tbody"></tbody></table></div>