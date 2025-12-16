---
title: Projects
updated: 2025-12-16 15:25:33Z
created: 2022-11-21 16:33:13Z
---

# :open_file_folder: Projects
###### t
A project is something to work on.
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: -tag:dedimo tag:.project.status.archive
fields: title
alias: title AS Project
sort: title ASC
details:
  open: false
  summary: Archived projects - {{count}}
-->
<details close>
<summary>Archived projects - 0</summary>

| Project |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: -tag:dedimo tag:.project -tag:.project.status.*
fields: title
alias: title AS Project
sort: title ASC
details:
  open: false
  summary: Projects without status - {{count}}
-->
<details close>
<summary>Projects without status - 0</summary>

| Project |
| --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
Tag: `.project`



## Kanban
```kanban
filters:
  tag: .project
columns:
  - name: Backlog
    tag: .project.status.backlog
  - name: Active
    tag: .project.status.active
```
Backlog | Active
--- | ---

_Last updated at 12/16/2025, 4:25:32 PM by Kanban plugin_