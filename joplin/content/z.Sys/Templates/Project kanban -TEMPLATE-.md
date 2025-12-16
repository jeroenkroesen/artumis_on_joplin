---
title: Project kanban -TEMPLATE-
updated: 2025-12-16 15:45:45Z
created: 2023-03-04 09:42:12Z
tags:
  - template
---

---
project_naam:
  label: naam
  type: text
project_tag:
  label: Tag (pr. prepended)
  type: text
project_status: dropdown(active, backlog, archive, permanent)
template_title: {{ project_naam }} -pr-
template_tags: .project, pr.{{ project_tag }}, .project.status.{{ project_status }}
template_notebook: 4804c5156b10432c89e3879d523737f9

---
# {{ project_naam }}
###### t
DELETE_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: type:note -tag:.project -tag:media tag:pr.{{ project_tag }}
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
search: tag:media tag:pr.{{ project_tag }}
fields: title
alias: title AS Media
sort: title ASC
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

[⬆️](#t)
***
[Projects](../../1.Mind/Projects.md)
Tag: `pr.{{ project_tag }}`



# Kanban
```\kanban
filters:
  tag: pr.{{ project_tag }}
  completed: false
columns:
  - name: Backlog
    backlog: true
  - name: Doing
    tag: todo.doing
  - name: Done
    tag: todo.done
```
Requests | Backlog | WIP
--- | --- | ---

_Last updated at 10/14/2024, 4:11:22 PM by Kanban plugin_