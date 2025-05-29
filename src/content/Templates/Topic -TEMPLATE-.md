---
title: Topic -TEMPLATE-
updated: 2025-03-20 15:49:51Z
created: 2023-08-20 11:49:32Z
tags:
  - template
---

---
topic_naam:
  label: Topic
  type: text
topic_tag:
  label: Tag (t. prepended)
  type: text
template_title: {{ topic_naam }} -t-
template_tags: topic, t.{{ topic_tag }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ topic_naam }}
##### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:topic tag:t.{{ topic_tag }}
fields: title
alias: title AS Topic
sort: title ASC
details:
  open: false
  summary: Related topics - \{\{count\}\}
-->
<details close>
<summary>Related topics - \{\{count\}\}</summary>

| Topic |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:topic -tag:media -tag:communication tag:t.{{ topic_tag }}
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
search: -tag:topic tag:media tag:t.{{ topic_tag }}
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
search: tag:communication tag:t.{{ topic_tag }}
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



| LinkTags | Tagging |
|-|-|
| [Topic](../1.Mind/Topic.md) | `t.{{ topic_tag }}` |
[⬆️](#t)
***
<br>