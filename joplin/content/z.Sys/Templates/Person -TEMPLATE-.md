---
title: Person -TEMPLATE-
updated: 2025-12-16 15:55:27Z
created: 2025-12-16 15:54:11Z
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
template_tags: person, p.{{ firstname_for_tag }}_{{lastname_for_tag}}, l.earth
template_notebook: 4804c5156b10432c89e3879d523737f9

---
# {{ firstname }} {{ lastname }}
###### t
DELETE_BACKSLASHES


|                | |
|------------------|---|
| Firstname     :| {{ firstname }} |
| Lastname      :| {{ lastname }} |
| Phone         :|  |
| Email         :|  |
| Street        :|  |
| House Number  :|  |
| Postal code   :|  |
| City          :|  |
| Province      :|  |
| Country       :|  |
| Planet        :| [Earth](:/aed6df3bb1fe433cb4c01dd45520ba6b) |
| Date of Birth :|  |
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: type:note -tag:person -tag:media tag:p.{{firstname_for_tag }}_{{lastname_for_tag}}
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
fields: title
alias: title AS Todo
sort: title ASC
details:
  open: false
  summary: Todo - \{\{count\}\}
-->
<details close>
<summary>Todo - \{\{count\}\}</summary>

| Todo |
| --- |
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

[⬆️](#t)
***
[Person](../../1.Mind/Person.md)
Tag: `p.{{ firstname_for_tag }}_{{lastname_for_tag}}`
