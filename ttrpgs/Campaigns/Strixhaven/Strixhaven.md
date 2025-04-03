---
world: Strixhaven
campaign: Strixhaven
status: active
role: GM
system: 
type: world
---
# The World of Strixhaven

## Player Characters


```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "player") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```


## Sessions
```meta-bind-button
label: New Session
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: command
    command: quickadd:choice:1442fd36-6dcc-4de4-a871-fb445f6937b1

```

```dataview
table summary as "Summary" from "ttrpgs/Strixhaven"
where contains(type,"session")
SORT sessionNum ASC
```


## Truths about the campaign/world

*Write down some facts about this campaign or the world that the characters find themselves in.*

## NPC's
```meta-bind-button
label: Add New Non Player Character
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: command
    command: quickadd:choice:bf10e7ec-f0f4-4fe7-96ec-889c5131754b

```

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", Race, Class
FROM "ttrpgs"
WHERE (NoteIcon = "npc") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```

## Factions
```meta-bind-button
label: New Faction
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: command
    command: quickadd:choice:a995968b-ee00-44cb-897e-ee92f5259337
```

```dataview
TABLE description as "Description" from "ttrpgs"
WHERE contains(lower(type),"faction")
WHERE (campaign = "Strixhaven")
```

## Custom rules

- [[Character options]]
- [[ttrpgs/Strixhaven/House Rules|House Rules]]

## [[Safety Tools]]