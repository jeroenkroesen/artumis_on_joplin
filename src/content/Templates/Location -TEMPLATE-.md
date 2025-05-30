---
title: Location -TEMPLATE-
updated: 2025-05-30 12:25:05Z
created: 2024-07-31 10:35:42Z
tags:
  - template
---

---
location_name:
  label: Name
  type: text
location_name_for_tag:
  label: Tag (l. prepended)
  type: text
template_title: {{ location_name }}
template_tags: location, l.{{ location_name_for_tag }}, l.earth
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ location_name }} 
###### t
DELETE_BACKSLASHES


| | |
|---|---|
| Containing locations :| `Tag locations that this location is in` |
| Location type(s) :|  |
| GPS coördinates :|  |
| Phone :|  |
| Email :|  |
| Street :|  |
| House Number :|  |
| Postal code :|  |
| City :|  |
| Province :|  |
| Country :|  |
| Planet :| [Earth](../1.Mind/Earth.md) |
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:location tag:l.{{ location_name_for_tag }}
fields: title, image
alias: title AS Location, image AS Pic
sort: title ASC
details:
  open: false
  summary: Locations inside this location - \{\{count\}\}
-->
<details close>
<summary>Locations inside this location - \{\{count\}\}</summary>

| Location | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:person tag:l.{{ location_name_for_tag }}
fields: title, image
alias: title AS Person, image AS Pic
sort: title ASC
details:
  open: false
  summary: Persons connected - \{\{count\}\}
-->
<details close>
<summary>Persons connected - \{\{count\}\}</summary>

| Person | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:organization tag:l.{{ location_name_for_tag }}
fields: title, image
alias: title AS Organization, image AS Pic
sort: title ASC
details:
  open: false
  summary: Organizations - \{\{count\}\}
-->
<details close>
<summary>Organizations - \{\{count\}\}</summary>

| Organization | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:person -tag:organization -tag:location -tag:media
  tag:l.{{ location_name_for_tag }}
fields: title, image
alias: title AS Note, image AS Pic
sort: title ASC
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
search: tag:media tag:l.{{ location_name_for_tag }}
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
<br>



| LinkTags | Tagging |
|-|-|
| [Location](../1.Mind/Location.md) | `l.{{ location_name_for_tag }}` |
[⬆️](#t)
***
<br>