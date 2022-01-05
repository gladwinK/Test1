# init
-to initialise git in a directory.
```
git init
```
# add

	-to add files/dir to staging.
	- 'git add fileName/directoryName'
	- 'git add -A'
	- 'git add .' (to add everything in current dir.).
# status
	-to get status of our repo.
	- 'git status'
	- 'git status -s' for summary of status( RED-M -> modified unstaged file GREEN-M -> staged but uncommited file).
	- GREEN-A -> NewFile which is staged but not commmited.
	- RED-?? -> NewFile which hasn't been staged yet.

# checkout
	-to change the working-directory to the latest staging 
		- 'git checkout fileName' replaces the working-directory file with the staged-file.
		- 'git checkout -f' replaces all the staged files compared to the latest commit.
		- the untracked files are unstirred.
	-to change the current branch
		- 'git checkout branchName'
	-to create a branch and move into it 
		- 'git checkout -b branchName'
# log
	-to see all the commits done with author-name, time, commit-message.
``` 
	'git log' 
```
	- 'git log -p -numberOfPreviousLogs'

# diff
	-shows difference in the staging and working-directory.
		- 'git diff'
	-can also show the difference in the last commit and current stage
		- 'git diff --staged'
	- --output='FileName' writes the output onto the file instead of stdout.
# commit
	-to move everything from staging to COMMIT.
	- 'git commit' this opens a file in vim editor so that you can write the commit-message.
	- 'git commit -m "message"' this will not open the prompt.
	- 'git commit -a' will directly add the untracked files and commit ( NOTE: Untracked and NOT a newFile).
# rm
	-to remove from staging
		- 'git rm --cached fileName'
	-to remove from staging and delete from the wroking-directory.
		- 'git rm fileName'
		
# restore
	- to unstage 'git restore --staged'
		

## .gitignore
	- to ignore file/directory.
	
	-create '.gitingore' in root directory of the git-init.
	-then configure it 
		- 'fileName.ext' to ignore a specific filename throughout all the directory/sub-directory.
		- '*.ext' to ignore all the files with .ext extensions.
		- '/filename.ext' to ignore the file only from root dir.
		- '/dir/fileName.ext' to ignore the specific file from a specific dir.
 
# branch
	-to create a branch
		- 'git branch branchName'
	-to create a branch and switch to it in one command
		- 'git checkout -b branchName'.	
# merge
	-first switch to the branch in which you want a merge a branch.
	-then 'git merge branchName'
 


### global ### config
	-to set - 'git config --global user.name/email 'userName'
	-to show - 'git config --global user.name/email'  
### remote
	- to add an origin - 'git remote add origin 'url'.
	- to show remote url - 'git config --get remote.origin.url'.
	- to set remote url -  'get remote set-url origin '{ newUrl}'. 

