---
title: Inline references query -SNIPPET-
updated: 2025-05-30 12:16:47Z
created: 2025-05-30 12:15:56Z
---

---
topic_naam:
  label: naam
  type: text
topic_tag:
  label: Tag (ref prepended)
  type: text
template_notebook: 490fbb213d6047daa4e360593536ff89

---
DELETE_BACKSLASHES
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