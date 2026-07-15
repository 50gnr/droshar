---
{"dg-publish":true,"dg-path":"4-Party/Sho.md","permalink":"/4-party/sho/","tags":["player","character","party"],"dg-note-properties":{"type":"vercel-character","aliases":null,"tags":["player","character","party"],"source":"[[ShoSlovak Trogaro]]"}}
---


# ShoSlovak Trogaro

> [!infobox|no-t right]  
> # ShoSlovak Trogaro  
> ![ShoSlovak Trogaro.png](/img/user/Assets/Images/Party/ShoSlovak%20Trogaro.png)
> ###### Character Details  
> Type | Stat  
> ---|---  
> Player | Josh  
> Level | 10  
> Class | Warlock  
> Subclass | —  
> Race | Human  
> Status | Alive  
> Age | `= this.source.char_age`  
> HP | `= this.source.hp` / `= this.source.max_hp`  
> AC | `= this.source.ac`  
> Passive Perception | 1
> Affiliation | [[Compendium/Lore/Organizations/The Lotus Choir\|The Lotus Choir]] 
> Languages | Common 


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




# ShoSlovak Trogaro


> [!infobox|no-t right]
> ![Assets/Images/Party/ShoSlovak Trogaro.png\|ShoSlovak Trogaro.png](/img/user/Assets/Images/Party/ShoSlovak%20Trogaro.png)
> ###### Details:
> | Type | Stat |
> | ---- | ---- |
> | :FasCrown: Level   | 10 |
> | :RiSwordFill: Class |  Warlock|
> | :FasUserShield: Archetype |  `=this.char_subclass`|
> |  :FasUserGroup: Race |  Human|
> | :FasArrowsUpDownLeftRight: HP | `=this.hp`


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
> > > ![[Compendium/Party/Player Characters/Player Facing/Sho#Skills\|no-h clean]]
> >
> > > ![[Compendium/Party/Player Characters/Player Facing/Sho#Inventory\|no-h1 clean]]
> >
> > > [!div-m|no-title]
> > > ![[Compendium/Party/Player Characters/Player Facing/Sho#Connections\|no-h1 clean]]
> > 
> > > [!div-m|no-title]
> > > ![[Compendium/Party/Player Characters/Player Facing/Sho#Relationships\|no-h1 clean]]



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

The following items belong to ShoSlovak Trogaro.

Items: `INPUT[inlineListSuggester(optionQuery(#Category/Quest)):char_items]`


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
    at eval (plugin:digitalgarden:90:61)</pre>mermaid", "flowchart LR", `Current[${current}]`];

parents.forEach((p, i) => {
  lines.push(`P${i}[${label(p)}] --> Current`);
});

partner.forEach((p, i) => {
  lines.push(`Current --> PT${i}[${label(p)}]`);
});

children.forEach((c, i) => {
  lines.push(`Current --> C${i}[${label(c)}]`);
});

siblings.forEach((s, i) => {
  lines.push(`Current --> S${i}[${label(s)}]`);
});

allies.forEach((a, i) => {
  lines.push(`Current --> A${i}[${label(a)}]`);
});

enemies.forEach((e, i) => {
  lines.push(`Current --> E${i}[${label(e)}]`);
});

lines.push("```");

dv.paragraph(lines.join("\n"));
```

# Faction Standing

<div><table class="dataview table-view-table"><thead class="table-view-thead"><tr class="table-view-tr-header"><th class="table-view-th"><span>Faction</span></th><th class="table-view-th"><span>Your Standing</span></th><th class="table-view-th"><span>Benefits</span></th><th class="table-view-th"><span>Primary Contact</span></th></tr></thead><tbody class="table-view-tbody"></tbody></table></div>

</div></div>


---

## Known Items

| Known Items |
| ----------- |
| \-          |

{ .block-language-dataview}

---

> [!column|flex 3]
>> [!important]- QUESTS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected Quests
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Party/Quests")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
>> ```
>
>> [!example]- GROUPS
>> ```base
>> properties:
>>   file.name:
>>     displayName: Name
>> views:
>>   - type: table
>>     name: Connected Groups
>>     filters:
>>       and:
>>         - file.inFolder("Compendium/Groups")
>>         - file.hasLink(this.file)
>>     order:
>>       - file.name
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
>>     order:
>>       - file.name
>> ```