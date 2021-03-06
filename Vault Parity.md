# Vault Parity
In order to set up a good documentation system for the [[Dashboard|game design vault]] (gdv) we will be using [obsidian git](https://github.com/denolehov/obsidian-git) to automatically commit, push, and pull all of the contents of the vault. However, incase seperate users would like to have seperate plugin folders, or just custom workflows, details of this setup are useful

## Requirements
1. Git is installed
2. Git bash settup allowed for 3rd party wrappers[^1]
3. The user is logged in
4. The user has a clone of the remote repository

The plugin should have all default settings cloned from the repo.

## Custom Settings
Inside the .gitignore file is a list of every file to be ignored git. `.obsidian/plugins/obsidian-git/data.json` contains the settings pertaining to how *obsidian git*  works. Most importantly, the ability to turn off notifications and change back up times. [^2]

To add more plugins to this list add `.obsidian/plugins/<plugin-name>/data.json` to the `.gitignore` file and it should allow users to customize their settings.

## Github Edits
If there are further changes to how the repo is managed, they should be changed in the [[README]], so it is easily viewed on the site if need be. 

```ad-warning
title: Future Changes
Removal of the .gitignore file will push any custom settings to the remote repo, meaning all users will automatically pull settings that they had previously customized! Don't do!
```
---
```ad-abstract
title: References
- [Obsidian Git](https://github.com/denolehov/obsidian-git) - Plugin info
- [Stackoverflow](https://stackoverflow.com/questions/35150667/how-to-ignore-a-directory-from-pull-on-remote-repository) - Ensured that .gitignore doesn't stop files from being pulled from remote 
```

[^1]: [Why git may not work at first](https://github.com/denolehov/obsidian-git/wiki/Installation#git-installation)
[^2]: This is very finnicky right now