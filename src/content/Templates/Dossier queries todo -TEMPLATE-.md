---
title: Dossier queries todo -TEMPLATE-
updated: 2025-03-26 16:20:55Z
created: 2024-12-31 15:59:33Z
tags:
  - template
---

---
dossier_naam:
  label: naam
  type: text
dossier_tag:
  label: Tag (t. prepended)
  type: text
dossier_status: dropdown(active, backlog, archive, permanent)
template_title: {{ dossier_naam }} -d-
template_tags: topic, dossier, t.{{ dossier_tag }}, dossier.{{ dossier_status }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
DELETE_BACKSLASHES


<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:t.{{ dossier_tag }} tag:todo.doing
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
search: type:todo iscompleted:0 tag:t.{{ dossier_tag }} tag:todo.backlog
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
search: type:todo iscompleted:0 tag:t.{{ dossier_tag }} tag:todo.done
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