[[Research Meetings]] %% tags:: #MOC %% 

# Meetings MOC
A meeting MOC is a <u>map of content</u> for meeting notes in Obsidian. Obsidian is a note-taking app that allows you to create and link notes in various ways. A meeting MOC is a page that helps you to organize and access your meeting notes, as well as create new ones with a template. A meeting MOC can also display information from your meeting notes using plugins such as Dataview and Meta Bind

A meeting MOC can help you to keep track of your tasks, goals, projects, and reflections for each meeting, as well as the date and attendees of the meeting. A meeting MOC can also help you to move important information from your meeting notes to more permanent notes in your vault.

**Template:** [[Meeting]]

```meta-bind-button
label: New Meeting
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Template/Meeting.md
    folderPath: Research diary/Meeting
    fileName: MSO
    openNote: true

```

## Meeting Notes

```dataview
TABLE file.cday as Created, summary
FROM "Research diary/Meeting" and -#MOC
SORT file.cday DESC
```