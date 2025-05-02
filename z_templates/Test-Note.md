<%*
const filePath = tp.file.path;
const tag = await tp.system.prompt("Enter tag to add:");
if (tag) {
    const existingTags = await tp.frontmatter.get("tags");
    const updatedTags = existingTags ? [...existingTags, tag] : [tag];
    await tp.frontmatter.set("tags", updatedTags);
}
%>