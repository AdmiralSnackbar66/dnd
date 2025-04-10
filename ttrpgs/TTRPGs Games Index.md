---
aliases:
  - games
banner_y: 0.86
banner: "![[games-banner.png]]"
---
# [[TTRPGs Games Index]]

## List of current campaigns

```meta-bind-button
label: Add New World
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
    command: quickadd:choice:2909bec8-1788-4692-bd75-a4925cb913e2
```

```dataviewjs
let totalGames;
function getNumOfGames(campaign) {
	let numOfGames = app.plugins.plugins.dataview.api
        .pages(`"ttrpgs/${campaign}"`)
        .where(page => {
            if (page.type === 'session') {
                if (page.campaign === campaign) {
	                totalGames = totalGames +1;
                    return true;
                }
            }
        }).length
	return numOfGames
}

dv.table(["Campaign","System","Sessions", "Role","Status"],dv.pages('"ttrpgs"')
  .where(b => b.type === "world")
  .sort(b => b.status)
  .map(b => [dv.fileLink(b.file.path,false,[b.campaign]),b.system,getNumOfGames(b.campaign),b.role,b.status]))
```

## List of  Player Characters

```meta-bind-button
label: Add New Player Character
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
    command: quickadd:choice:83f21e4b-1d22-461c-9318-4ac66025c1f8
```

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", campaign, Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "player") 
SORT file.mtime DESC
```

## List of Non Player Characters

```meta-bind-button
label: Add New NPC
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
TABLE WITHOUT ID link(file.name) AS "Name", campaign, Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "npc") 
SORT file.mtime DESC
```