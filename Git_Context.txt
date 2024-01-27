/*

GIT:Version control System

Types of Repositories:

	1.	RemoteRepository
	2.	LocalRepository
	3.	WorkingRepository	

Types of states:

	1.	Untrackingstate:

	2.	Trackingstate:
		1.	Modifiedstate
		2.	staggedstate
	
*/

-----------------------------------------------------------------------------------------------------------------------


commands:

Help: 

	git command -h	: 	will display all the commands that associated with that command.
	

Clone:

	git clone URL	: 	Cloning the Project from the RemoteRepository to WorkingRepository.
	
Initializing: Initializing the git to the particular folder that not containg git.

	git init		:	Git will initialize to that folder.
	
RemoteConnection:	Connecting to the RemoteRepository.

	git remote add remotename RemoteURL		: Connection will establish in between the WorkingRepository to RemoteRepository	
	
	
Add: add the untracked files or modified files to the staggedstate. 
	
	git add filename		: 	add particular file to the staggedstate.

	git add .				: 	add all files to the staggedstate.
	
	
Commit: Save the changes happend in the WorkingRepository to the LocalRepository.

	git commit				: 	Type the message and save it.
	
	git commit -v			:	Save the file along with changes happend.
	
	git commit -m "Message"	: 	Inline commit along with Message.
	

Push:	Push the files from WorkingRepository to RemoteRepository.

	git push origin master	:	Push to the RemoteRepository master branch.
	
fetch:	pull the files from RemoteRepository to LocalRepository.

	git fetch				:	Changes will come to the LocalRepository only not to the WorkingRepository.
	
merge: pull the files from LocalRepository to WorkingRepository.
	
	git merge				:	pull the files that saved in LocalRepository to the WorkingRepository.
	
pull:	Combination of both fetch&merge. pull the files from LocalRepository to WorkingRepository in a single step.

	git pull 				: 	LocalRepository -> WorkingRepository
	
.gitignore:	Concept to ignore the unrequired files for this we need create gitignore file and need to add the files init.
	1.	filename
	2.	*.txt
	3.	foldername/
	4.	!file.txt


diff: To find difference between commits.


	git diff							: 	Will gives all the difference in between staged and WorkingRepository.
	
	git diff Commitid 					: 	will gives the difference between last staged and commitid.
	
	git diff firstcommitid nextcommitid :	will gives the difference between the firstcommitid & nextcommitid.
	
	stat	: only status will provide.
	
	filename: only gives data related that filename.

	--Ex	:	git diff Firstcommitid NextCommitid --stat filename.txt
	
	
	Nocommitid	: Modified & Staged(last commitid)
	
	commitid1	: Modified & commitid1
	
	Commitid2	: Commitid2 & Commitid1
	
	
	git difftool	:	will show case the difference in side by side.
	
	
	
	
status:	will gives the Information of state of the file whether its tracked or untracked, Modified or Committed.

	git status		:
	
	
log (History) :	To get the Commits of the working directory.

	git log :
	
	git log -number : only specified number commits only will display.
	
	git log filename: will gives the commits that correlated to that filename.
	
	

	git log --pretty=ssoneline:
	
	git log --pretty=full :
	
	git log --pretty=short :
	
	git log --pretty=fuller :
	
	git log --oneline --graph --all :
	
	
show :	To check the actual change of the commit.

	git show commitid:	will gives the all the changes happend in that commit.
	
	git show commitid --stat: status of the changes.
	
	git show commitid filename:	specified filename data only will display.
	
	git show commitid --stat filename:	status of the specified filename changes.
	
	
alias:	renameing the command or giving the alias name to the command.

	git config --global alias.allcommits "log --oneline --graph -- all"
	
-----------------------------------------------------------------------------------------------------------------------
	
	
Branch: Git branch is nothing but a pointer pointing to separate location.

	git branch	: To get the branch names
	
	git branch -a: all brances in that Git.
	
	git branch branchname:	Creating a new branch with branchname.
	
	git checkout branchname	:	Shifting to that branch.
	
	git checkout -b branchname : Create & shift at a command.
	
	git branch -d branchname : Deleting a branch.
	
	git merge branchname : merging a branch into other main branch.
	
	
Merge: Commanly there are two types of merge.

	1. Fast-Farword Merge
	2. Recursive Merge
	
	Fast-farword Merge	:	If there is no commits happend after the branching then it will come as under Fast-Farword Merge.
	
	Recursive Merge : If any commits happend parllarly with branch commints in master then it will be come under Recursive Merge.
	
	
	
	git branch --merge : To check wt branches are merged.
	
	git branch --no-merge : To check wt branches are not merged yet.
	
	
-----------------------------------------------------------------------------------------------------------------------
	
	
	
	
	

	





