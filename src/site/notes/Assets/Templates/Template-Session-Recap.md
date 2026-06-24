---
{"dg-publish":true,"permalink":"/assets/templates/template-session-recap/","tags":["session","recap","Category/Journal"],"dg-note-properties":{"type":"session-recap","session_number":null,"session_title":null,"session_date":null,"arc":"C2 Southern Principalities","players":null,"OneLiner":null,"tags":["session","recap","Category/Journal"],"obsidianUIMode":"preview"}}
---


<%*
const title = tp.file.title;
const match = title.match(/session\s*(\d+)/i);
const sessionNum = match ? match[1].padStart(2, "0") : await tp.system.prompt("Session number?");
const cleanTitle = `Session ${sessionNum} - Recap`;

if (tp.file.title !== cleanTitle) {
  await tp.file.rename(cleanTitle);
}

await app.fileManager.processFrontMatter(tp.config.target_file, fm => {
  fm["session_number"] = Number(sessionNum);
  fm["session_title"] = `Session ${sessionNum}`;
});

// Set Iconize icon
const iconize = app.plugins.plugins["obsidian-icon-folder"];
if (iconize) {
  const file = tp.file.find_tfile(cleanTitle);
  if (file) {
    iconize.addFolderIcon(file.path, "FasBookOpen");
    iconize.api?.util?.dom?.createIconNode?.(iconize, file.path, "FasBookOpen");
  }
}
%>

# Session <% sessionNum %> - Recap

> [!quote]
> `= this.OneLiner`

## Summary



---

## Major Events

- 

---

## Important Discoveries

- 

---

## Notable NPCs

- 

---

## Important Locations

- 

---

## Rewards & Treasures

- 

---

## Looking Ahead



# Hidden Data

## DM Notes

