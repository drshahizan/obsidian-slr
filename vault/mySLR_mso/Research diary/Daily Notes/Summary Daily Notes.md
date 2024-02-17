
[[Summary Daily Notes]] %% tags:: #DN %% 

Summary daily notes are notes that you create in Obsidian to summarize your day, such as what you did, learned, achieved, or enjoyed. Summary daily notes can help you to reflect on your progress, goals, and challenges, as well as to capture any insights or ideas that you might have. Summary daily notes can also help you to link your daily activities to your other notes in Obsidian, such as projects, tasks, or resources.

**Template:** [[Daily]]


## Notes

```dataview
TABLE file.cday as Created, topic
FROM "Research diary/Daily Notes" and -#DN
SORT file.cday DESC
```