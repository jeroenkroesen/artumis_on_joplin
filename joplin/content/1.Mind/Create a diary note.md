---
title: Create a diary note
updated: 2025-03-26 16:29:43Z
created: 2025-03-25 22:11:51Z
tags:
  - howto
  - t.artumis_learn_second_brain
  - t.artumis_second_brain
---

# Create a diary note
###### t



## 1. New note from template
Press `ctrl` +`shift`+`alt`+`n`. The dialog to make new note from a template appears. From the dropdown, select the template `Diary Day` and click `OK` or press the `enter` key. 
![Screenshot from 2025-03-20 23-25-25.png](../_resources/Screenshot%20from%202025-03-20%2023-25-25.png)
[⬆️](#t)
***
<br>



## 2. Fill out template fields and create note
Use `leading zero` (ie: `03`, not ~~3~~) notation for the following fields:
* Month_numeric
* Week_nr
* Day_nr

Use 4 digits for the year. Write month names in English without any capital letters.
![Screenshot from 2025-03-20 23-34-09.png](../_resources/Screenshot%20from%202025-03-20%2023-34-09.png)

Click `OK` or press the `enter` key.
[⬆️](#t)
***
<br>



## 3. Add the snippet `insertbody` to the first note query
In the diary note select and delete the text `INSERTHERE`

With the cursor in place of the deleted text press `ctrl`+`alt`+`i`.  The dialog to insert a template in an existing note appears. Choose the template `insertbody -TEMPLATE-` and press `OK
[⬆️](#t)
***
<br>



## 4. Delete all backslashes
Press `ctrl`+`h` to open the `find and replace` dialog.  Replace `\`  with nothing by clicking the button `(all)`
![Screenshot from 2025-03-20 23-36-08.png](../_resources/Screenshot%20from%202025-03-20%2023-36-08.png)

Lastly, delete the reminder text `REMOVE_BACKSLASHES_INSERT_BODY_TEMPLATE` from the note.
[⬆️](#t)
***
<br>



## 5. Find your diary notes
Diary notes for the current day, current week, next week and last week are automatically linked to the start note: [(1).Start](../1.Mind/%281%29.Start.md) if they are labelled correctly with `time.` tags. Diary notes are automatically time tagged if you create them with the `Diary Day` template and fill out the fields correctly.

It may take up to 5 minutes for a new diary note to appear on the start page. To force a refresh, press `F7` or open the `Tools` menu and choose `Update note overview`.
[⬆️](#t)
***
<br>



## 5. Write
To quickly start writing anything in your diary, just put the cursor under the line `###### tt` and start writing.

If you want write a longer piece of diary, with one or more headings, put the cursor in the empty space above the first note overview query (the text that begins with `<!-- note-overview-plugin`). You can start a heading (I advise level 2 headings inside a diary note) by typing two hashtags `##` followed by a space and your heading text.

To close a diary entry with heading, copy and paste the text below under it, or insert the template snippet titled `Toplink - line - break` (press `ctrl`+`alt`+`i` to insert a template in an existing note).
```
[⬆️](#t)
***
<br>
```

In the howto [Connect an idea to a topic](../1.Mind/Connect%20an%20idea%20to%20a%20topic.md) we will dive deeper into organizing your diary.
[⬆️](#t)
***
<br>

[Artumis Second Brain -t-](../1.Mind/Artumis%20Second%20Brain%20-t-.md) - [Learn Artumis Second Brain -d-](../1.Mind/Learn%20Artumis%20Second%20Brain%20-d-.md)

| LinkTags |
|-|
| [Howto](../1.Mind/Howto.md) |
[⬆️](#t)
***
<br>