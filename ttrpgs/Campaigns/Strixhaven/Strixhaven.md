---
world: Strixhaven
campaign: Strixhaven
status: active
role: GM
system: 5e
type: world
---

# The World of [[Strixhaven]]

## Player Characters

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "player") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```

## Sessions

```dataview  
TABLE date,status, summary
FROM "ttrpgs"
WHERE (type = "session") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```

## Truths about the campaign/world

*Write down some facts about this campaign or the world that the characters find themselves in.*

## NPC's

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", Race, Class
FROM "ttrpgs"
WHERE (NoteIcon = "npc") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```

## Factions

```dataview
TABLE description as "Description" from "ttrpgs"
WHERE contains(lower(type),"faction")
WHERE (campaign = "Strixhaven")
```

## Locations

```dataview  
TABLE WITHOUT ID link(file.name) AS "Location"
FROM "ttrpgs/Campaigns/Strixhaven/Locations"
WHERE (NoteIcon = "location") 
WHERE (campaign = "Strixhaven")
SORT file.mtime DESC
```


## Custom rules

- [[Character options]]
- [[ttrpgs/Strixhaven/House Rules|House Rules]]

## [[Safety Tools]]