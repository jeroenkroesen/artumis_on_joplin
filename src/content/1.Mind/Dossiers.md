---
title: Dossiers
updated: 2025-03-26 21:06:53Z
created: 2025-03-10 19:00:10Z
tags:
  - concept
---

# :open_file_folder: Dossiers
###### t
A dossier is something to work on. It differs from a [Topic](../1.Mind/Topic.md) because a dossier is mainly ment to organize todo's and track progress, whereas a topic is ment to gather any information related to that topic.

There are 2 templates for dossiers: 
[Dossier kanban](../Templates/Dossier%20kanban%20-TEMPLATE-.md)
Includes a Kanban board
[Dossier simple](../Templates/Dossier%20simple%20-TEMPLATE-.md)
Does *not* include a Kanban board
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:dossier.permanent
fields: title
alias: title AS Dossier
sort: title ASC
details:
  open: true
  summary: Permanent dossiers - {{count}}
-->
<details  open>
<summary>Permanent dossiers - 0</summary>

| Dossier |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:dossier.archive
fields: title
alias: title AS Dossier
sort: title ASC
details:
  open: false
  summary: Archived dossiers - {{count}}
-->
<details close>
<summary>Archived dossiers - 0</summary>

| Dossier |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:dossier -tag:dossier.*
fields: title
alias: title AS Dossier
sort: title ASC
details:
  open: false
  summary: Dossiers without status - {{count}}
-->
<details close>
<summary>Dossiers without status - 0</summary>

| Dossier |
| --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
<br>



| Tagging |
|-|
| `dossier` |
[⬆️](#t)
***
<br>



## Kanban
```kanban
filters:
  tag: dossier
columns:
  - name: Backlog dossiers
    tag: dossier.backlog
  - name: Active dossiers
    tag: dossier.active
```
Backlog dossiers | Active dossiers
--- | ---
|  | [Learn Artumis Second Brain -d-](../1.Mind/Learn%20Artumis%20Second%20Brain%20-d-.md) |
_Last updated at 3/26/2025, 10:06:31 PM by Kanban plugin_