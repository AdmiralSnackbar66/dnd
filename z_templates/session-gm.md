---
type: session
campaign: <% tp.file.folder(false) %>
world: <% tp.user.getThisWorld(tp) %>
sessionNum: <% tp.user.getThisGameNum(tp) %>
location: 
date: <% tp.date.now("YYYY-MM-DD") %>
fc-category:
  - Sessions
long_rest: false
short_rest: false
summary: ""
tags:
  - prep
art: ""
---
# [[<% tp.file.title %>]]

## Session Summary

> [!tldr] [[<% tp.file.title %>]]
>  ^summary

---

## Housekeeping



## Recap

![[<% tp.user.getLastGameTitle(tp) %>#^summary]]

## Review The Characters
%%
>[!tip] Review the Characters
>Before we do anything else, it helps to spend a few minutes reviewing the player characters.  What are their names? What do they want? What plays into their backgrounds? What do the players of these characters enjoy to do at the table?
>
>You might not even write anything down during this step, but reviewing the characters helps wire them into your mind - and ensures that the rest of your preparation fits around them.
%%
 ```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, Race, Class, ac, pasperc As "Pass Perc (WIS)"
from "ttrpgs"
where contains(Role, "Player") 
where contains(campaign, "<%tp.file.folder(false)%>")
```


## Strong start

> 

## Scenes

- [ ] 
- [ ] 
- [ ] 
- [ ] 

## Secrets and Clues

- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 

## Fantastic locations

- [ ] 
- [ ] 
- [ ] 
- [ ] 
- [ ] 

## Potential Monsters

- [ ] 
- [ ] 
- [ ] 
- [ ] 

## Potential Treasure

- [ ] 
- [ ] 

---

## Log

