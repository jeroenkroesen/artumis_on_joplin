---
title: Category -TEMPLATE-
updated: 2025-12-16 15:43:34Z
created: 2025-05-17 13:01:18Z
tags:
  - template
---

---
category_naam:
  label: Category
  type: text
category_tag:
  label: Tag (c. prepended)
  type: text
template_title: {{ category_naam }} -c-
template_tags: .category, c.{{ category_tag }}
template_notebook: 4804c5156b10432c89e3879d523737f9

---
# {{ category_naam }}
##### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:.topic tag:c.{{ category_tag }}
fields: title, image
alias: title AS Topic, image AS Pic
sort: title ASC
details:
  open: true
  summary: Topics - \{\{count\}\}
-->
<details  open>
<summary>Topics - \{\{count\}\}</summary>

| Topic | Pic |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:.topic -tag:media tag:c.{{ category_tag }}
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
search: tag:media tag:c.{{ category_tag }}
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
[Category](../../1.Mind/Category.md)
Tag: `c.{{ category_tag }}`