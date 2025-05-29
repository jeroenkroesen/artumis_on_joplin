---
title: Diary day -TEMPLATE-
updated: 2025-03-20 22:38:54Z
created: 2024-08-18 20:10:41Z
latitude: 52.19448960
longitude: 4.41910120
altitude: 0.0000
tags:
  - template
---

---
Year: text
Month_numeric: text
Month_name: text
Week_number: text
Day_number: text
Day_name: text
template_title: {{ Year }}-{{ Month_numeric }}-{{ Day_number }} {{Day_name}} Diary
template_tags: diary, time.{{ Year }}, time.{{ Month_name }}, time.week_{{ Week_number }}, time.day_{{ Day_number }}
template_notebook: 724417f57c0947c488f5dd4167652d67

---
# {{ Day_number }}-{{ Month_numeric }}-{{ Year }} {{Day_name}}
###### tt
REMOVE_BACKSLASHES_INSERT_BODY_TEMPLATE

[⬆️](#tt)
***
<br>



<!-- note-overview-plugin
search: type:note -tag:communication* -tag:appointment -tag:media
  tag:time.{{Year}} tag:time.{{Month_name}} tag:time.day_{{Day_number}}
fields: body
listview:
  text: INSERTHERE
-->
<!--endoverview-->

<!-- note-overview-plugin
search: type:note tag:time.{{Year}} tag:time.{{Month_name}} tag:time.day_{{Day_number}}
fields: title
alias: title AS Notes
sort: title ASC
details:
  open: true
  summary: Notes - \{\{count\}\}
-->
<details  open>
<summary>Notes - \{\{count\}\}</summary>

| Notes |
| --- |
</details>
<!--endoverview-->

<!-- note-overview-plugin
search: type:todo iscompleted:0 tag:todo.doing tag:time.{{Year}}
  tag:time.{{Month_name}} tag:time.day_{{Day_number}}
fields: title
alias: title AS Todo
sort: title ASC
details:
  open: true
  summary: Todo - \{\{count\}\}
-->
<details  open>
<summary>Todo - \{\{count\}\}</summary>

| Todo |
| --- |
</details>
<!--endoverview-->

[⬆️](#tt)
***
<br>



| LinkTags |
|-|
| [Diary](../1.Mind/Diary.md) |
[⬆️](#tt)
***
<br>