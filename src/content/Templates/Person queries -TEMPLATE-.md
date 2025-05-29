---
title: Person queries -TEMPLATE-
updated: 2025-03-20 15:49:22Z
created: 2024-12-20 15:30:52Z
tags:
  - template
---

---
firstname:
  label: First name
  type: text
lastname:
 label: Last name
 type: text
firstname_for_tag:
  label: First name for tag (lowercase and underscores, p. prepended)
  type: text
lastname_for_tag:
 label: Last name for tag (lowercase and underscores)
 type: text
template_title: {{ firstname }} {{ lastname }}
template_tags: person, p.{{ firstname_for_tag }}_{{lastname_for_tag}}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
DELETE_BACKSLASHES

<!-- note-overview-plugin
search: type:note -tag:person -tag:media -tag:communication tag:p.{{
  firstname_for_tag }}_{{lastname_for_tag}}
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
search: tag:person tag:p.{{ firstname_for_tag }}_{{lastname_for_tag}}
fields: title, image
alias: title AS Person, image AS Pic
sort: title ASC
details:
  open: false
  summary: Persons - \{\{count\}\}
-->
<details close>
<summary>Persons - \{\{count\}\}</summary>

| Person | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:p.{{ firstname_for_tag }}_{{lastname_for_tag}}
fields: title, tags
alias: title AS Todo, tags AS Context
sort: title ASC
details:
  open: false
  summary: Todo - \{\{count\}\}
-->
<details close>
<summary>Todo - \{\{count\}\}</summary>

| Todo | Context |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:media tag:p.{{ firstname_for_tag }}_{{lastname_for_tag}}
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

<!-- note-overview-plugin
search: tag:communication tag:p.{{ firstname_for_tag }}_{{lastname_for_tag}}
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