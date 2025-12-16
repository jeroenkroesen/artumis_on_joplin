---
title: Topic -TEMPLATE-
updated: 2025-12-16 15:46:43Z
created: 2023-08-20 11:49:32Z
tags:
  - template
---

---
topic_naam:
  label: Topic
  type: text
topic_tag:
  label: Tag (t. prepended)
  type: text
template_title: {{ topic_naam }} -t-
template_tags: .topic, t.{{ topic_tag }}
template_notebook: 4804c5156b10432c89e3879d523737f9

---
# {{ topic_naam }}
##### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: type:note -tag:.topic -tag:media tag:t.{{ topic_tag }}
fields: title, image
alias: title AS Note, image AS Pic
sort: title DESC
details:
  open: false
  summary: Notes - \{\{count\}\}
-->
<details close>
<summary>Notes - \{\{count\}\}</summary>

| Note | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:media tag:t.{{ topic_tag }}
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

<br>

<!-- note-overview-plugin
search: tag:.project tag:t.{{ topic_tag }} tag:.project.status.active
fields: title
alias: title AS Project
sort: title DESC
details:
  open: false
  summary: Active Projects - \{\{count\}\}
-->
<details close>
<summary>Active Projects - \{\{count\}\}</summary>

| Project |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:.project tag:t.{{ topic_tag }} tag:.project.status.backlog
fields: title
alias: title AS Project
sort: title DESC
details:
  open: false
  summary: Backlog Projects - \{\{count\}\}
-->
<details close>
<summary>Backlog Projects - \{\{count\}\}</summary>

| Project |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:.project tag:t.{{ topic_tag }} tag:.project.status.archive
fields: title
alias: title AS Project
sort: title DESC
details:
  open: false
  summary: Archived Projects - \{\{count\}\}
-->
<details close>
<summary>Archived Projects - \{\{count\}\}</summary>

| Project |
| --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
[Topic](../../1.Mind/Topic.md)
Tag: `t.{{ topic_tag }}`



## Kanban
```\kanban
filters:
  tags:
    - .project
    - t.{{ topic_tag }}
columns:
  - name: Backlog
    tag: .project.status.backlog
  - name: Active
    tag: .project.status.active
```
Backlog | Active
--- | ---

_Last updated at 10/20/2025, 12:23:02 AM by Kanban plugin_