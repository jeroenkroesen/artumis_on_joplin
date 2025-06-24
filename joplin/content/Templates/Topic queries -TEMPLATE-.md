---
title: Topic queries -TEMPLATE-
updated: 2025-05-30 12:40:07Z
created: 2025-03-09 19:12:02Z
tags:
  - template
---

---
topic_tag:
  label: Tag (t. prepended)
  type: text
template_tags: t.{{ topic_tag }}, topic

---

REMOVE_ALL_BACKSLASHES
REPLACE_NULL_WITH_REGEX

<!-- note-overview-plugin
search: ref_{{ topic_tag }}
fields: title, excerpt
listview:
  text: |-
    
    \{\{title\}\}
    \{\{excerpt\}\}
excerpt:
  regex: null
  regexflags: gmi
  removenewline: false
  removemd: false
details:
  open: false
  summary: Inline references - \{\{count\}\}
-->
<details close>
<summary>Inline references - \{\{count\}\}</summary>

</details>
<!--endoverview-->

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
search: tag:media tag:t.{{ topic_tag }}
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