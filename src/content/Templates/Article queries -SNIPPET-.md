---
title: Article queries -SNIPPET-
updated: 2025-05-30 12:03:06Z
created: 2025-05-30 11:56:04Z
tags:
  - template
---

---
article_tag:
  label: Tag (a. prepended)
  type: text
template_tags: a.{{ article_tag }}, .article
template_notebook: 490fbb213d6047daa4e360593536ff89

---
<!-- note-overview-plugin
search: tag:article tag:a.{{ article_tag }}
fields: title
alias: title AS Article
sort: title ASC
details:
  open: false
  summary: Related articles - \{\{count\}\}
-->
<details close>
<summary>Related articles - \{\{count\}\}</summary>

| Article |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:note -tag:media -tag:article -tag:communication tag:a.{{ article_tag }}
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
search: -tag:article tag:media tag:a.{{ article_tag }}
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
search: tag:communication tag:a.{{ article_tag }}
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