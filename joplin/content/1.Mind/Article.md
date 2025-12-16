---
title: Article
updated: 2025-12-16 15:37:50Z
created: 2023-04-08 20:43:51Z
tags:
  - .concept
---

# :scroll: Article
###### t
A longer piece of writing by me.

Tag articles with these state tags:
`.article.state.backlog` - I'd like to write this article or complete it
`.article.state.wip` - Writing is in progress
`.article.state.unpublished` - The article is done, but not published
`.article.state.published` The article is done and published
[⬆️](#t)
***
<br>



<!-- note-overview-plugin
search: tag:.article tag:.article.state.wip
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
search: tag:.article tag:.article.state.backlog
fields: title
alias: title AS Article
sort: title ASC
details:
  open: false
  summary: Backlog - {{count}}
-->
<details close>
<summary>Backlog - 0</summary>

| Article |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: tag:.article tag:.article.state.unpublished
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
search: tag:.article tag:.article.state.published
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
search: tag:.article -tag:.article.state.*
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
[Concept](../1.Mind/Concept.md)
Tag: `.article`