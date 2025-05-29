# Artumis on Joplin
Implementing the Artumis second brain method in the Joplin note-taking app.  
  
[Artumis](https://jeroenkroesen.github.io/artumis_site/)
***

# CHANGELOG

***

## Branche 'zen_interface'
When comparing Joplin to Obsidian and LogSeq, the Joplin UI comes across as dated, stale and a little cluttered. A second brain should have a clean, peaceful zen vibe. It is already possible to hide the sidebar and note list with default shortcuts.  
  
The following remained in the way of clutter:
* Menu bar
* Tab bar
* Markdown bar
* Buttons at the right of the markdown bar  
  
I'm talking about all this clutter at the top:  
![cluttered Joplin](/.resources/cluttered.png)  
  
Luckily a lot can be accomplished by editing `userchrome.css`. Check out this beautiful zen version of Joplin:  
![cluttered Joplin](/.resources/uncluttered.png)  
  
Ofcourse by hiding UI, functionality is lost. The functionality I truly missed I've added back through shortcuts: Settings alarms and viewing note properties.  
  
  

### Keyboard shortcuts
* Added: `Ctrl+Alt+Q` to view note properties
* Added: `Ctrl+Alt+A` to set or edit an alarm on a todo
* Added: `Ctrl+Alt+O` to toggle the tab bar

### Interface (userchrome)
* Hide: rightside button bar (note-title-info-group)
* Hide: markdown toolbar (CodeMirrorToolbar)
