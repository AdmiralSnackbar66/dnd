---
obsidianUIMode: preview
---


> [!cards|4]
> **[[Map-Faerun]]**
> [![[Northern Faerun Map.jpg\|sban htiny ctr]]](Lampoteuo)
> 
> **[[Link]]**
> [![[JourneyBoard.png\|sban htiny ctr]]](Journey%20Board)
>
> **[[Link]]**
> [![[AdventureIcon.png\|sban htiny ctr]]](Lampoteuo)
> 
> **[[Link]]**
> [![[PartyLogo.jpg\|sban htiny ctr p+t]]|](Party%201%2FExample%20Party%201)

# Sessions

> [!infobox]
> # Session Journals
> ```dataview
TABLE WITHOUT ID link(file.name) AS "Session Date", Status, players
from "3-Session Journals"
where (type = "Session Journal")
where (sessionstatus="Complete")
SORT file.name DESC

# Party Members

```meta-bind-button
label: Add New Party Member
hidden: false
id: ""
style: primary
actions:
  - type: templaterCreateNote
    templateFile: "z_Templates/TemplatePartyMember.md"
    fileName: NewPartyMember
```

```dataview  
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, Class, Race, level, Role  
from "2-Party"  
where (Role = "Player")  
where (Status = "Active")  
```

# Recently Modified NPCs

```meta-bind-button
label: New NPC
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
TABLE WITHOUT ID link(file.name) AS "NPC Name", Gender, Race, Age, Location, AssociatedGroup  
FROM "3-Mechanics/NPC's"
WHERE (NoteIcon = "npc") 
SORT file.mtime DESC
LIMIT 10
```


# Recently Modified Locations

```dataview  
TABLE WITHOUT ID link(file.name) AS "Location Name", type, Government, Community-Size, size, population  
FROM "4-World"
WHERE (NoteIcon = "Settlement")  
SORT file.mtime DESC
LIMIT 10
```


# Recently Modified Notes
```dataview
TABLE WITHOUT ID
    link(file.path, file.folder + " / " + file.name) AS "Note",
    file.mtime AS "Last modified"
FROM "/"
WHERE file.mtime >= date(today) - dur(30 days)
AND file.name != this.file.name
    AND !contains(file.path, "z_Assets")
    AND !contains(file.path, "Inline Scripts")
    AND !contains(file.path, "z_Templates")
    AND !contains(file.path, "daily notes")
    AND !contains(file.path, "BRAT")
SORT file.mtime DESC
LIMIT 10
```

![[Vault Report]]


