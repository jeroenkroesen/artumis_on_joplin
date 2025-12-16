---
title: Diary day -TEMPLATE-
updated: 2025-12-16 15:48:56Z
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
template_tags: .diary, time.{{ Year }}, time.{{ Month_name }}, time.week_{{ Week_number }}, time.day_{{ Day_number }}
template_notebook: 7cf44aa247d641cd95a62fdfe15fb4e2

---
# {{ Day_number }}-{{ Month_numeric }}-{{ Year }} {{Day_name}}
###### t
REMOVE_BACKSLASHES_INSERT_BODY_TEMPLATE

[⬆️](#tt)
***
<br>



<!-- note-overview-plugin
search: type:note -tag:.appointment -tag:event.birthday -tag:media
  tag:time.{{Year}} tag:time.{{Month_name}} tag:time.day_{{Day_number}}
fields: body
listview:
  text: INSERT_BODY
-->
<!--endoverview-->

<!-- note-overview-plugin
search: type:note tag:time.{{Year}} tag:time.{{Month_name}} tag:time.day_{{Day_number}}
fields: title, image
alias: title AS Notes, image AS Pic
sort: title ASC
details:
  open: true
  summary: Notes - \{\{count\}\}
-->
<details  open>
<summary>Notes - \{\{count\}\}</summary>

| Notes | Pic |
| --- | --- |
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
[Diary](../../1.Mind/Diary.md) - LINK_TO_YEAR