# Vault Parity
In order to set up a good documentation system for the [[gdv|game design vault]] (gdv)we will be using [obsidian git](https://github.com/denolehov/obsidian-git) to automatically commit, push, and pull all of the contents of the vault. However, incase seperate users would like to have seperate plugin folders, or just custom workflows, details of this setup are useful

## Requirements
1. Git is installed
2. The user is logged in
3. The user has a clone of the remote repository

The plugin should have all default settings cloned from the repo.

## Custom Settings
Inside the .gitignore file is a list of every file to be ignored git. `.obsidian/plugins/obsidian-git/data.json` contains the settings pertaining to how *obsidian git*  works. Most importantly, the ability to turn off notifications and change back up times.

To add more plugins to this list add `.obsidian/plugins/<plugin-name>/data.json` to the `.gitignore` file and it should allow users to customize their settings.

```ad-warning
title: Future Changes
Removal of the .gitignore file will push any custom settings to the remote repo, meaning all users will automatically pull settings that they had previously customized! Don't do!
```
---
```ad-abstract
title: References
- [Obsidian Git](https://github.com/denolehov/obsidian-git) - Plugin info
- [Stackoverflow](https://stackoverflow.com/questions/35150667/how-to-ignore-a-directory-from-pull-on-remote-repository) - Ensured that no 
Author: 
```