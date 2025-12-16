---
title: Project simple -TEMPLATE-
updated: 2025-12-16 15:46:11Z
created: 2023-03-04 09:35:23Z
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
##### t
DELETE_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:pr.{{ project_tag }} tag:todo.doing
fields: title
alias: title AS Todo
sort: title ASC
details:
  open: false
  summary: Doing - \{\{count\}\}
-->
<details close>
<summary>Doing - \{\{count\}\}</summary>

| Todo |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:pr.{{ project_tag }} -tag:.issue*
fields: title
alias: title AS Todo
sort: title ASC
details:
  open: false
  summary: Backlog - \{\{count\}\}
-->
<details close>
<summary>Backlog - \{\{count\}\}</summary>

| Todo |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:pr.{{ project_tag }} tag:todo.done
fields: title
alias: title AS Todo
sort: title ASC
details:
  open: false
  summary: Done - \{\{count\}\}
-->
<details close>
<summary>Done - \{\{count\}\}</summary>

| Todo |
| --- |
</details>
<!--endoverview-->

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
[Project](../../1.Mind/Projects.md)
Tag: `d.{{ project_tag }}`