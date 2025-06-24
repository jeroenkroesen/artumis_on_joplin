---
title: Category -TEMPLATE-
updated: 2025-05-30 12:05:48Z
created: 2025-05-30 12:03:32Z
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
template_tags: category, c.{{ category_tag }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ category_naam }}
##### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:topic tag:c.{{ category_tag }}
fields: title
alias: title AS Topic
sort: title ASC
details:
  open: false
  summary: Topics - \{\{count\}\}
-->
<details close>
<summary>Topics - \{\{count\}\}</summary>

| Topic |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:topic -tag:media -tag:communication tag:c.{{ category_tag }}
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

<!-- note-overview-plugin
search: tag:communication tag:c.{{ category_tag }}
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



| Tagging |
|-|
`c.{{ category_tag }}` |
[⬆️](#t)
***
<br>