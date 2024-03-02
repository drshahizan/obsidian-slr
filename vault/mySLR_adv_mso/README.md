
# Obsidian Vault for Systematic Literature Reviews in Computer Science

This repository hosts an Obsidian vault tailored for conducting a Systematic Literature Review (SLR). An SLR is a meticulous and transparent approach to synthesizing and evaluating existing literature related to a specific research question. Obsidian is a robust note-taking application that offers features such as linking, tagging, and graphing of notes. By utilizing GitHub, the vault can be synchronized, backed up, and shared with other researchers. GitHub is a web-based platform that hosts code repositories and offers version control, collaboration, and documentation capabilities. This vault template is intended for computer science researchers seeking to perform an SLR using Obsidian and GitHub.

## What you need to do  🚀

### 1. Install Zotero Plugin

#### a. Zotfile
ZotFile is a third-party plugin for Zotero that helps you manage your attachments, such as PDFs. It can automatically rename, move, and sync your files with your mobile device or cloud storage. It can also extract annotations from PDFs and save them as Zotero notes. Here are the steps to install and use ZotFile:

1. On the [ZotFile site]((https://zotfile.com/)), click **Download** and the **xpi file** will be downloaded. 
2. In the Zotero application, go to *Tools > Add-Ons*.
3. Click on the *gear icon* and choose *"Install Add-on from file"*   
4. Locate your downloaded xpi file and click Open
5. Restart Zotero and go to *Tools -> ZotFile Preferences* to configure the plugin settings according to your needs.
6. To use ZotFile, you can right-click on any Zotero item or attachment and select Manage Attachments from the menu. You will see various options to rename, move, send, or get files from your tablet or cloud service. You can also extract annotations from PDFs by selecting Extract Annotations.

For more details and examples, you can watch this [video tutorial](https://www.youtube.com/watch?v=faYJ4gEGZ40) or visit the [ZotFile website](http://zotfile.com) or the [GitHub repository](https://github.com/jlegewie/zotfile) for more information and support.

#### b. Better BibTeX
Better BibTeX is a plugin for Zotero that enhances its functionality for LaTeX users. It allows you to generate customized citation keys, export your library in BibTeX or BibLaTeX format, and sync your attachments with your tablet or cloud service. Here are the steps to install and use Better BibTeX:

1. Download the ‘Better BibTeX for Zotero’ plugin from [here](https://github.com/retorquere/zotero-better-bibtex/releases/tag/v6.7.36). Hover your cursor to `zotero-better-bibtex-6.7.36.xpi`, then right-click and select ‘Save link as’ to download the addon.
2. Open Zotero and go to *Tools -> Add-ons -> Tools for all Add-ons* (the small, drop-down wheel in the top right corner) *-> Install Add-on From File* and select the downloaded file.
3. Restart Zotero and go to *Tools -> Better BibTeX Preferences* to configure the plugin settings according to your needs.
4. To use Better BibTeX, you can right-click on any Zotero item or attachment and select Manage Attachments from the menu. You will see various options to rename, move, send, or get files from your tablet or cloud service. You can also extract annotations from PDFs by selecting Extract Annotations.
5. To export your library in BibTeX or BibLaTeX format, you can right-click on a collection or the whole library and select Export Collection. Then, choose Better BibTeX or Better BibLaTeX as the format and save the file.
6. To generate customized citation keys, you can use the Citation key formula option in the Better BibTeX Preferences. You can use various placeholders and modifiers to create your own pattern. For example, `[auth:lower]_[year]` will generate keys like `shahizan_2024`.
  
For more details and examples, read this [guide](https://tex.stackexchange.com/questions/702678/generating-citation-keys-with-zotero-and-better-bibtex-plugin).

### 2. Obsidian Plugins
Obsidian is a powerful note-taking app that allows you to create and link your notes in various ways. To enhance your note-taking experience, you can use plugins that add extra features and functionalities to Obsidian. The plugins used in this vault are as follows:

| No. | Plugins | Description |
| ---: | --- | --- |
| 1 | [Admonition](https://github.com/valentine195/obsidian-admonition) | A plugin that allows you to create block-styled admonitions (notes, warnings, tips, etc.) in your notes. |
| 2 | [Autocomplete](https://github.com/yeboster/autocomplete-obsidian) | A plugin that provides autocomplete suggestions for words, tags, links, and commands in your notes. |
| 3 | [Better Word Count](https://github.com/lukeleppan/better-word-count) | A plugin that shows the word count, character count, and reading time of your notes in the status bar. |
| 4 | [Calendar](https://github.com/liamcain/obsidian-calendar-plugin) | A plugin that adds a calendar view to your notes, where you can see and create notes based on dates. |
| 5 | [cMenu Plugin](https://github.com/chetachiezikeuzor/cMenu-Plugin) | A plugin that adds a customizable context menu to your notes, where you can access various commands and actions. |
| 6 | [Dataview](https://github.com/blacksmithgu/obsidian-dataview) | A plugin that allows you to query, filter, sort, and display data from your notes using a simple query language. |
| 7 | [Excalidraw](https://github.com/zsviczian/obsidian-excalidraw-plugin) | A plugin that integrates Excalidraw, a tool for creating hand-drawn diagrams, into your notes. |
| 8 | [Iconize](https://github.com/FlorianWoelki/obsidian-icon-folder) | A plugin that lets you add icons to your folders and notes in the file explorer. |
| 9 | [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) | A plugin that generates a reference list from your citations using Pandoc. |
| 10 | [Kanban](https://github.com/mgmeyers/obsidian-kanban) | A plugin that allows you to create and manage kanban boards in your notes. |
| 11 | [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration) | A plugin that integrates Zotero, a tool for managing bibliographic data, into your notes. |
| 12 | [Charts](https://github.com/phibr0/obsidian-charts) | This plugin lets you create editable, interactive and animated charts in Obsidian via Chart.js. You can use different types of charts, such as pie, bar, line, radar, etc., and customize them with various options. | 
| 13 | [Chartview](https://github.com/caronchen/obsidian-chartsview-plugin) | This plugin is another data visualization solution in Obsidian, based on Ant Design Charts. It supports plots and graphs, such as word cloud, treemap, dual axes, mix, organization tree graph, etc. You can also import data from external or internal CSV files, or use dataviewjs to generate data. | 
| 14 | [Pandoc Plugin](https://github.com/OliverBalfour/obsidian-pandoc) | This plugin allows you to export your notes to a variety of formats using Pandoc, a command-line tool for document conversion. You can export to formats such as Word, PDF, ePub, HTML, PowerPoint, LaTeX, and many more. You can also use Pandoc templates and citations to customize your output. | 
| 15 | [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) | This plugin displays a formatted reference in the sidebar for each Pandoc citekey present in the current document. It uses Pandoc to generate the reference style, and you can choose from thousands of CSL styles. You also need to supply a compatible bibliography file, such as a .bib or .json file. |

These plugins can help you make your notes more organized, informative, and creative. You can install them from the Obsidian community plugins page or from their GitHub repositories.

To check for updates for your plugins, please follow these steps:
1. Go to **Settings → Community plugins → Current plugins**.
2. Click on the **Check for updates** button. You will update all plugins.