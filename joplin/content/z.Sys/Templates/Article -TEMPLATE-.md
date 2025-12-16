---
title: Article -TEMPLATE-
updated: 2025-12-16 15:43:04Z
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
template_title: {{ article_name }} -a-
template_tags: a.{{ article_tag }}, .article
template_notebook: 4804c5156b10432c89e3879d523737f9

---
# {{ article_name }}
###### t
REMOVE_ALL_BACKSLASHES

[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:.article tag:a.{{ article_tag }}
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
search: type:note -tag:media -tag:.article tag:a.{{ article_tag }}
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
search: -tag:.article tag:media tag:a.{{ article_tag }}
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



| Writing start | Published date |
|---------------|----------------|
| DD-MM-YYYY    | -              |
[⬆️](#t)
***
[Article](../../1.Mind/Article.md)
Tag: `a.{{ article_tag }}`