---
title: Location queries -TEMPLATE-
updated: 2025-05-30 12:25:05Z
created: 2025-01-01 18:58:06Z
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
template_tags: location, l.{{ location_name_for_tag }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
DELETE_BACKSLASHES

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