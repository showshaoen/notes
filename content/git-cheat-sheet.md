---
title: Git Cheat Sheet
draft: false
tags: 
enableToc: true
---
[Install Git](https://git-scm.com/downloads)
# Initialize Git on a new device
1. Set up username and email
	```bash
	git config --global user.name "YOUR_USERNAME" 
	git config --global user.email "YOUR_EMAIL"
	```
2. Change current directory to the project folder, right click and select 'Git Bash Here' or use the Command Prompt.
3. Initialize the local directory as a git repository
	```bash
	git init
	```
4. Add files to the new local repository. This stages them for the first commit. ('.' means all the files/folders in the directory)
	```bash
	git add .
	```
5. Commit the files that were staged to the local repository. (-m for message)
	```bash
	git commit -m "First commit"
	```
6. To push to a remote repository, for example GitHub, first create a new repository on GitHub.
7. Push the local repository to GitHub.
	```bash
	# Creates a connection between local repo and remote repo on GitHub
	git remote add origin https://github.com/showshaoen/fyp-web.git
	# Changes main branch's name to 'main'
	git branch -M main
	# Pushes the repo from local device to GitHub
	git push -u origin main
	```

# Clone an Existing Repository
1. Choose a local directory, right click, then select 'Git Bash Here'.
2. Clone the repo using a url.
	```bash
	git clone https://github.com/showshaoen/iz-app.git
	```
3. Change directory into the project folder.
	```bash
	cd iz-app
	```
4. Fetch all remote branches and refs to synchronize.
	```bash
	git fetch origin -v -a
	```
5. Commit to main branch as usual
	```bash
	git commit -m "Test commit"
	```
6. Can also set up a new branch
	```bash
	git checkout -b "<new_branch_name>"
	git push --set-upstream origin "<new_branch_name>" 
	```

# Useful Commands
## Branches
- List all existing branches
	```bash
	git branch -a
	```
- Switch HEAD branch
	```bash
	git checkout <branch_name>
	```
- Create a new branch based on current HEAD
	```bash
	git branch <new_branch_name>
	```
- Delete a local branch
	```bash
	git branch -d <branch_name>
	```
## Commit History and Local Changes
- Show all commits, starting with newest
	```bash
	git log
	```
- Show changes over time for a specific file
	```bash
	git log -p <filename>
	```
- Who changed what and when in a file
	```bash
	git blame <filename>
	```
- Changed files in working directory
	```bash
	git status
	```
- Changes to tracked file
	```bash
	git diff
	```
- Add all current changes to the next commit
	```bash
	# Add/stage all files which has been modified/delete, including untracked file
	git add .
	# Add/stage tracked files only which has been modified/deleted
	git add -u
	```