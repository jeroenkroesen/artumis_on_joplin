---
title: Dossier kanban -TEMPLATE-
updated: 2025-03-26 16:20:34Z
created: 2023-03-04 09:42:12Z
tags:
  - template
---

---
dossier_naam:
  label: Naam
  type: text
dossier_tag:
  label: Tag (t. prepended)
  type: text
dossier_status: dropdown(active, backlog, archive, permanent)
template_title: {{ dossier_naam }} -d-
template_tags: topic, dossier, t.{{ dossier_tag }}, dossier.{{ dossier_status }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ dossier_naam }}
###### t
DELETE_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:issue tag:t.{{ dossier_tag }}
fields: title
alias: title AS Issue
sort: title DESC
details:
  open: false
  summary: Issues - \{\{count\}\}
-->
<details close>
<summary>Issues - \{\{count\}\}</summary>

| Issue |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:media -tag:communication tag:t.{{ dossier_tag }}
fields: title
alias: title AS Note
sort: title DESC
details:
  open: false
  summary: Notes - \{\{count\}\}
-->
<details close>
<summary>Notes - \{\{count\}\}</summary>

| Note |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:media tag:t.{{ dossier_tag }}
fields: title
alias: title AS Media
sort: title DESC
details:
  open: false
  summary: Media - \{\{count\}\}
-->
<details close>
<summary>Media - \{\{count\}\}</summary>

| Media |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:communication tag:t.{{ dossier_tag }}
fields: title
alias: title AS Communication
sort: title DESC
details:
  open: false
  summary: Communication - \{\{count\}\}
-->
<details close>
<summary>Communication - \{\{count\}\}</summary>

| Communication |
| --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
<br>



| LinkTags | Tagging |
|-|-|
| [Dossiers](../1.Mind/Dossiers.md) | `t.{{ dossier_tag }}` |
[⬆️](#t)
***
<br>



# Kanban
```\kanban
filters:
  tag: t.{{ dossier_tag }}
  completed: false
columns:
  - name: Backlog
    tag: todo.backlog
  - name: Doing
    tag: todo.doing
  - name: Done
    tag: todo.done
```
Requests | Backlog | WIP
--- | --- | ---

_Last updated at 10/14/2024, 4:11:22 PM by Kanban plugin_