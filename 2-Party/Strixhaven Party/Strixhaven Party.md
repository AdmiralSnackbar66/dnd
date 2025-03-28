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
from "2-Party/Strixhaven Party"
where (Role = "Player")
where (Status="Active")
```

<br>

```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name", Player,hp, ac, modifier, pasperc As "Passive Perception (WIS)"
from "2-Party/Strixhaven Party"
where (Role = "Player") 
where (Status = "Active") 
```

