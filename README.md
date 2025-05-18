# Introduction

This workflow incorporates two Universal Actions which act on a file or files selected in Finder. Both prompt you to create a new folder. One then *moves* the selected file(s) to that folder. The other *copies* the file(s) to that folder. 

Note that if you intend most of the time to create new folders in a single, unchanging base folder you can check, in the workflow configuration, `Use a default base folder for all new folders` and then select the default base folder in the folder picker below that. That will save you having to select the base folder on every occasion you wish to move or copy files to a new sub-folder of that default.

# Usage

1. Simply select a file or files in Finder, press your Universal Action hotkey (<kbd>⌘ /</kbd> by default) and, if this workflow title does not appear at the top of the list of your Universal Actions, start typing a word from the name of this workflow until you see the name of this workflow.

![UA](https://github.com/user-attachments/assets/35ab062a-942f-4f1c-af52-295423ecde79)

2. Unless you are using a default base folder (in which case this step will be skipped) choose the folder in which you wish to create the new folder. Just start typing the name of the folder to see a list of matching folders from which you can select the appropriate one. (See also the important note below about discovery of folders.)

![BaseFolder](https://github.com/user-attachments/assets/4ed15e96-6ab8-46d0-8b7b-a40773d77a35)

3. After pressing <kbd>↩︎</kbd> on the highlighted folder you will be prompted for the name of the new folder.

![NewFolder](https://github.com/user-attachments/assets/11f908e2-e288-49f7-ab17-b48d7d3818c0)

When you press <kbd>↩︎</kbd> the new folder will be created and the file or files moved (or copied) to it—with a notification to confirm what has happened.

# Important notes
- In order for a folder to be found in the second step of the workflow *it must be within your default search scope*. (See `Alfred Preferences → Features → Default Results` and look under `Search Scope`.) However, if you want to be able to find folders outside that scope just double click on the workflow `File Filter`, go to `Scope` and drag in the folder(s) you wish to be included within the file filter search scope. *Note that if you do that you'll also as well have to drag in the folders that are within your Alfred search scope*. If you don't do that the folder search will be limited only to the new folders you have dragged in.
- The sound can be muted in the configuration (see the checkbox opposite).
- If there already exists in the destination folder a folder with the same name as that you have proposed you will be warned and must end the workflow. In other words, this workflow will not overwrite an existing folder.

# Acknowledgement

I am indebted to @sepulchra on the [Alfred forum](https://www.alfredforum.com/) for the provocation to write the original workflow but, particularly, for invaluable help and advice developing and testing that workflow.
