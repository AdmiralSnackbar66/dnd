---
noteIcon: NPC
aliases:
  - Movinder
pronouns: she/her
role: NPC
statBlock: 
role_internal: Year 1 Guidance councillor and a professor of Radiance
species: 
personality: 
motivation: 
associatedGroups: 
associatedCharacters: 
importantItems: 
description: Silverquills Professor of Radiance, seeks to inspire greatness in all that they do, pushing their students to look for the good in all things and bring that into the light.
---
# `=this.file.name`
`=this.file.description`

>[!div-m|grid-m]
>
>>[!div-m]
>>| Key                   | Value                        |
>>| --------------------- | ---------------------------- |
>>| Aliases:              | `=this.aliases`              |
>>| Pronouns:             | `=this.pronouns`             |
>>| Species:              | `=this.species`              |
>>| Role:                 | `=this.role_internal`        |
>>| Personality:          | `=this.personality`          |
>>| Motivation:           | `=this.motivation`           |
>>| Associated Groups:    | `=this.associatedGroups`     |
>>| AssociatedCharacters: | `=this.associatedCharacters` |
>>| Important Items:      | `=this.importantItems`       |
>
>>[!div-m]
>>![[ImagePlaceholder.png|500]]
>
>>[!div-m]
>>```dataviewjs
>>const codeBlock = "```"
>>const part1 = `statblock
>>name: `;
>>const part2 = `
>>monster: `;
>>const part3 = `
>>columns: 1
>>`;
>>const name = dv.current().file.name;
>>const frontmatter = dv.markdownList(dv.current().file.frontmatter).toString().split("-");
>>let monster;
>>for (i = 0; i < frontmatter.length; i++){
>>	if (!frontmatter[i].includes("statBlock")) continue;
>>	monster = frontmatter[i].split(":")[1].slice(1);
>>	break;}
>>const markdown = codeBlock + part1 + name + part2 + monster + part3 + codeBlock;
>>dv.paragraph(markdown)
>>```