---
title: Article -TEMPLATE-
updated: 2025-03-20 15:48:20Z
created: 2024-10-14 10:32:44Z
tags:
  - template
---

---
article_name:
  label: Title
  type: text
article_tag:
  label: Tag (a. prepended)
  type: text
template_title: {{ article_name }}
template_tags: article, a.{{ article_tag }}
template_notebook: 490fbb213d6047daa4e360593536ff89

---
# {{ article_name }}
###### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:article tag:a.{{ article_tag }}
fields: title, tags
alias: title AS Article, tags AS Context
sort: title ASC
details:
  open: true
  summary: Related articles - \{\{count\}\}
-->
<details  open>
<summary>Related articles - \{\{count\}\}</summary>

| Article | Context |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: -tag:media -tag:article -tag:communication tag:a.{{ article_tag }}
fields: title, tags
alias: title AS Note, tags AS Context
sort: title DESC
details:
  open: true
  summary: Notes - \{\{count\}\}
-->
<details  open>
<summary>Notes - \{\{count\}\}</summary>

| Note | Context |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: -tag:article tag:media tag:a.{{ article_tag }}
fields: title, tags
alias: title AS Media, tags AS Context
sort: title ASC
details:
  open: true
  summary: Media - \{\{count\}\}
-->
<details  open>
<summary>Media - \{\{count\}\}</summary>

| Media | Context |
| --- | --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:communication tag:a.{{ article_tag }}
fields: title, tags
alias: title AS Communication, tags AS Context
sort: title DESC
details:
  open: true
  summary: Communication - \{\{count\}\}
-->
<details  open>
<summary>Communication - \{\{count\}\}</summary>

| Communication | Context |
| --- | --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
<br>



| LinkTags | Writing start | Published date  | Tagging |
|-|-|-|-|
| [Article](../1.Mind/Article.md) | DD-MM-YYYY | - | `a.{{ article_tag }}` |
[⬆️](#t)
***
<br>