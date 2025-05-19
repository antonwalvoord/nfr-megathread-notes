---
dg-publish: true
---
# TLDR;
There are a lot of things that you can set up to make editing nice, but the bare root of things is that this wiki is written as a collection of markdown files that link to one another. All you really need is access to the [[#Permissions|GitHub repository for the notes]] and to edit those notes in some text editor of your choice. I personally recommend Obsidian but it doesn't really matter.

You'll have to pull the files from the GitHub and then once you've made your edits to the notes push your files to the GitHub and then message Anton to have them published to the website.
# Obsidian
Obsidian is what I use to edit the megathread and I highly recommend it. It stores files locally so you can edit/view them offline. It also has incredible support for plugins, 4 of which I use extensively and have setup information for below.
- Download Obsidian [here](https://obsidian.md/download)

After installing Obsidian, launch it and create a new vault called "MEGATHREAD" in a file location of your choice. Don't add any files to the vault yet. Then set up the plugins below (Git is mandatory, the others are extremely useful).

**Note:** in order to edit the megathread, you'll need [[#Permissions|permissions]]
#### Plugins
##### Git (Mandatory)
In order to make sure everyone is operating off of a shared version we use Git for version control. Obsidian has a great plugin for this which makes it incredibly easy to stay in sync with the repo. **Whenever you finalize changes to the repo you must commit them and push them. DO NOT push them unless you are ready to have them published to the live version, as someone else will likely pull and then unknowingly publish your changes. To avoid this, make sure that all settings labelled "Auto commit-and-sync" are DISABLED** 
- If you don't have Git installed on your computer, reference [this guide](https://nfr-learn.ue.r.appspot.com/lessons/4/3/) steps **4 and 5**
- Go to the [Git](obsidian://show-plugin?id=obsidian-git) plugin page, install and enable it
- Follow [this guide](https://publish.obsidian.md/git-doc/Getting+Started) to fully set up the plugin
	- **Note:** On step 3 of the instructions, choose to do the option: `Move all your files from the new folder (including .git !) into your vault root.`
- When you clone the repository you should use [this](https://github.com/antonwalvoord/nfr-megathread-notes.git) link
	- **Note:** When you do so, make sure you specify a *relative* path instead of an absolute path. So instead of `C:\Users\blah-blah`, just type the name of the new folder you want to create.
- When using this plugin, the most useful command is "commit-and-sync". This command will automatically stage all your changes, commit them, then pull from remote to prevent merge conflicts, and finally push them to the remote repository. In order to use this command, use ctrl/cmd+p and type in "Git: Commit-and-sync"
	- **Tip:** typing in "sync" will autocomplete to this command, you can also set a hotkey for it in Obsidian's hotkey settings
- Ensure you have the setting "Pull on startup" turned **ON**
##### Imgur (Optional)
I have personally run into issues with embedding files and having them successfully upload to the site. If you run into those same issues (I think you likely will) you should install the Obsidian [Imgur](obsidian://show-plugin?id=obsidian-imgur-plugin) plugin. It automatically uploads images you paste into the doc to Imgur which works much better. Follow the setup guide on the install page.

If you need to embed other types of files, there are ways to do this through html as well [[FSAE 2025 Rules|See: FSAE 2024 Rules]]
##### Omnisearch
This plugin adds search functionality to search the entire vault, similarly to how the website search function works. It also has additional functionality for creating/opening files. Use [this](obsidian://show-plugin?id=omnisearch) link to install it
# Permissions
In order to edit the megathread you'll need to be added as a collaborator on the Git repository where the thread is housed. Contact Anton on [slack](https://nufsae.slack.com/team/U05U23W4WJV) or by [email](mailto:antonwalvoord2027@u.northwestern.edu) to be added.

You'll need to be added as a collaborator on [the notes repo](https://github.com/antonwalvoord/nfr-megathread-notes)
# Usage Notes
If you're going to be editing a portion of the megathread "owned" by another member (owned meaning they are in charge of it's content or it's highly relevant to them) you should contact them prior to pushing your changes.

In an attempt to keep a consistent style, please refer to the [[Style Guide]] for general formatting notes. **This file is unpublished and only available to editors, open in Obsidian/editor of your choice after cloning to view.**