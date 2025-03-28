---
world: Strixhaven
campaign: Strixhaven
status: active
role: GM
system: D&D 5e
type: world
---
# The World of Strixhaven

## Player Characters

- [[Elvis Parsley]]
- [[Roleck Nevari]]
- [[Zolon Orielson]]

## Sessions

*Put your cursor where the session link should be. Then, from the Command Palette (CMD/CTRL+P), select either QuickAdd: Macro - Add session-player or QuickAdd: Macro - Add session-gm*.

```dataview
table summary as "Summary" from "ttrpgs/Strixhaven"
where contains(type,"session")
SORT sessionNum ASC
```


## Truths about the campaign/world

*Write down some facts about this campaign or the world that the characters find themselves in.*

- The players will believe that [[ttrpgs/Strixhaven/Murgaxor Grenshel|Murgaxor Grenshel]] is the main villain as written in the published adventure however the main villain is actually [[ttrpgs/Strixhaven/Extus Narr|Extus Narr]] and [[ttrpgs/Strixhaven/The Oriq|The Oriq]]


## Factions

```dataview
TABLE description as "Description" from "ttrpgs/Strixhaven"
WHERE contains(lower(type),"faction")
```

## Custom rules

- [[Character options]]
- [[ttrpgs/Strixhaven/House Rules|House Rules]]

## [[Safety Tools]]