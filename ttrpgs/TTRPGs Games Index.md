---
aliases:
  - games
banner_y: 0.86
banner: "![[games-banner.png]]"
---
# [[TTRPGs Games Index]]

## List of current campaigns


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

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", campaign, Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "player") 
SORT file.mtime DESC
```

## List of Non Player Characters

```meta-bind-button
label: Add NPC
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
    command: quickadd:choice:bd9c1196-2f8e-490e-938e-e6ec765e13d6

```

```dataview  
TABLE WITHOUT ID link(file.name) AS "Name", campaign, Race, Class, ac, hp, pasperc
FROM "ttrpgs"
WHERE (NoteIcon = "npc") 
SORT file.mtime DESC
```