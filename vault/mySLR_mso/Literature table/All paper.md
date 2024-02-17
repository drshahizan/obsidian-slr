> [!NOTE] Explanation
> This is some Obsidian wizardry using the [plugin dataview.](https://github.com/blacksmithgu/obsidian-dataview) It requires some expertise to fully customize. But the idea is that you can qrite custom queries to your notes and filter only those that have specific meta data or tags in them. Here are a few examples. (If it does not work, go to settings, activate community plugins and add "dataview")

You can change the source code of the table to customize the table

```dataview
table title, authors, year, keywords, itemtype
from "Literature_collection"
sort year desc
```

