---
dg-publish: true
---
# Obsidian
Obsidian is what I use to edit the megathread and I highly recommend it. It stores files locally so you can edit/view them offline. It also has incredible support for plugins, 3 of which I use extensively and have setup information for below.
- Download Obsidian [here](https://obsidian.md/download)

After installing Obsidian, launch it and create a new vault called "MEGATHREAD" in a file location of your choice. Don't add any files to the vault yet. Then set up the plugins below (Git is mandatory, the others are extremely useful).
#### Plugins
##### Git (Mandatory)
In order to make sure everyone is operating off of a shared version we use Git for version control. Obsidian has a great plugin for this which makes it incredibly easy to stay in sync with the repo. **Whenever you finalize changes to the repo you must commit them and push them. DO NOT push them unless you are ready to have them published to the live version, as someone else will likely pull and then unknowingly publish your changes. To avoid this, make sure that all settings labelled "Auto commit-and-sync" are DISABLED**
- If you don't have Git installed on your computer, reference [this guide](https://nfr-learn.ue.r.appspot.com/lessons/4/3/) steps **4 and 5**
- Go to the [Git](obsidian://show-plugin?id=obsidian-git) plugin page, install and enable it
- Follow [this guide](https://publish.obsidian.md/git-doc/Getting+Started) to fully set up the plugin
- When you clone the repository you should use [this](https://github.com/antonwalvoord/nfr-megathread-notes.git) link
- When using this plugin, the most useful command is "commit-and-sync". In order to use this command, use ctrl/cmd+p and type in "Git: Commit-and-sync"
	- Tip: typing in "sync" will autocomplete to this command, you can also set a hotkey for it in Obsidian's hotkey settings
##### Digital Garden (Optional)
If you want to be able to publish to the site yourself you'll need this plugin, otherwise someone else with the plugin will need to pull your changes from GitHub and then publish
- Go to the [Digital Garden](obsidian://show-plugin?id=digitalgarden) plugin page, install and enable it
- You need to create an access token to your GitHub Account. This acts as a sort of password so that the plugin can add new notes to your GitHub repository on your behalf. Go to [this page](https://github.com/settings/tokens/new?scopes=repo) while logged in to GitHub. The correct settings should already be applied. (If you don't want to generate this every few months, choose the "No expiration" option.) Click the "Generate token" button, and copy the token you are presented with on the next page.
- Open Obsidian and the settings for "Digital Garden" and fill in your GitHub username, the name of the repo (nfr-megathread), and lastly paste in your token.
- Now you can publish to the site!
##### Imgur (Optional)
I have personally run into issues with embedding files and having them successfully upload to the site. If you run into those same issues (I think you likely will) you should install the Obsidian [Imgur](obsidian://show-plugin?id=obsidian-imgur-plugin) plugin. It automatically uploads images you paste into the doc to Imgur which works much better. Follow the setup guide on the install page.

# Permissions
In order to edit the megathread you'll need to be added as a collaborator on the Git repository where the thread is housed. Contact Anton on [slack](https://nufsae.slack.com/team/U05U23W4WJV) or by [email](mailto:antonwalvoord2027@u.northwestern.edu) to be added.

# Usage Notes
If you're going to be editing a portion of the megathread "owned" by another member (owned meaning they are in charge of it's content or it's highly relevant to them) you should contact them prior to pushing your changes.