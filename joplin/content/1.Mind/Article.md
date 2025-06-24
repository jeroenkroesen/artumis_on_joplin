---
title: Article
updated: 2025-03-26 21:05:11Z
created: 2025-03-10 19:00:08Z
tags:
  - concept
---

# :scroll: Article
###### t
A longer piece of writing by you.

Tag articles with these state tags:
`article.state.wip` - Writing is in progress
`article.state.unpublished` - The article is done, but not published
`article.state.published` - The article is done and published

Use the template [Article](../Templates/Article%20-TEMPLATE-.md) to create new articles.
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:article tag:article.state.wip
fields: title
alias: title AS Article
sort: title ASC
details:
  open: true
  summary: In progress - {{count}}
-->
<details  open>
<summary>In progress - 0</summary>

| Article |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:article tag:article.state.unpublished
fields: title
alias: title AS Article
sort: title ASC
details:
  open: false
  summary: Unpublished - {{count}}
-->
<details close>
<summary>Unpublished - 0</summary>

| Article |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:article tag:article.state.published
fields: title
alias: title AS Article
sort: title ASC
details:
  open: false
  summary: Published - {{count}}
-->
<details close>
<summary>Published - 0</summary>

| Article |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:article -tag:article.state.*
fields: title
alias: title AS Article
sort: title ASC
details:
  open: false
  summary: No state - {{count}}
-->
<details close>
<summary>No state - 0</summary>

| Article |
| --- |
</details>
<!--endoverview-->

[⬆️](#t)
***
<br>



| Tagging |
|-|
| `article` |
[⬆️](#t)
***
<br>