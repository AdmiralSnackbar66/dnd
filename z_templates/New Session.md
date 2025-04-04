---
sessionstatus:
  - planned
sessiondate: 01/01/2025 
campaign: 
noteicon: journal
tags:
  - session
sessionNum: <%tp.user.getThisGameNum%>
---
# <%tp.file.title%>

## Session Summary
>[!tldr]  [[<% tp.file.title %>]]
>^summary

## Recap
![[<%tp.user.getLastGameTitle(tp)%>#^summary]]

## Review The Characters
%%
>[!tip] Review the Characters
>Before we do anything else, it helps to spend a few minutes reviewing the player characters.  What are their names? What do they want? What plays into their backgrounds? What do the players of these characters enjoy to do at the table?
>
>You might not even write anything down during this step, but reviewing the characters helps wire them into your mind - and ensures that the rest of your preparation fits around them.
%%
 ```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name", Player, Race, Class, ac, pasperc As "Pass Perc (WIS)", choice(Field1, "☑", "☐") as Present
from "2-Party/Strixhaven Party"
where contains(Role, "Player") 
where contains(Status, "Active")
```

## Strong Start

