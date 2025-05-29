---
title: Organization -TEMPLATE-
updated: 2025-03-20 15:49:11Z
created: 2023-05-31 11:05:39Z
tags:
  - template
---

---
organization_name:
  label: Name
  type: text
organization_name_for_tag:
  label: Tag (o. prepended)
  type: text
template_title: {{ organization_name }}
template_tags: organization, o.{{ organization_name_for_tag }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ organization_name }}
###### t
DELETE_BACKSLASHES


|                  |  |
|--------------------|--|
| Primary contact :|  |
| Website         :|  |
| Phone           :|  |
| Email           :|  |
| Street          :|  |
| House Number    :|  |
| Postal code     :|  |
| City            :|  |
| Province        :|  |
| Country         :|  |
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:person tag:o.{{ organization_name_for_tag }}
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
search: type:note -tag:media -tag:person -tag:communication tag:o.{{
  organization_name_for_tag }}
fields: title
alias: title AS Note
sort: title ASC
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
search: tag:media tag:o.{{ organization_name_for_tag }}
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
search: tag:communication tag:o.{{ organization_name_for_tag }}
fields: title
alias: title AS Communication
sort: title ASC
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
| [Location](../1.Mind/Location.md) | `o.{{ organization_name_for_tag }}` |
[⬆️](#t)
***
<br>