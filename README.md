## Install Git

	sudo apt-get install git

## git config

	Sets configuration values for your user name, email, gpg key, preferred diff algorithm, file formats and more. Example:

	git config user.name "Billy Everyteen"
	# Set a new name
	git config user.name
	# Verify the setting
	Billy Everyteen

## git init

	Initializes a git repository – creates the initial ‘.git’ directory in a new or in an existing project.  
		
		cd /home/user/my_new_git_folder/ git init

## git clone

	Makes a Git repository copy from a remote source. Also adds the original location as a remote so you can fetch from it again and push to it if you have permissions. 
	 
		git clone git@github.com:user/test.git(git-url)

## git add

	Adds files changes in your working directory to your index.
	
		git add .

## git rm

	Removes files from your index and your working directory so they will not be tracked. 
	 
		git rm filename

## git commit

	Takes all of the changes written in the index, creates a new commit object pointing to it and sets the branch to point to that new commit. 

		git commit -m ‘committing added changes’
		git commit -a -m ‘committing all changes, equals to git add and git commit’

## git checkout

	Checks out a different branch – switches branches by updating the index, working tree, and HEAD to reflect the chosen branch.
		git checkout newbranch

## git branch

	Lists existing branches, including remote branches if ‘-a’ is provided. Creates a new branch if a branch name is provided.

		git branch -a * master remotes/origin/master

## git merge

	Merges one or more branches into your current branch and automatically creates a new commit if there are no conflicts.

		git merge newbranchversion

## git fetch

	Fetches all the objects from the remote repository that are not present in the local one.

		git fetch origin

## git pull

	Fetches the files from the remote repository and merges it with your local one. This command is equal to the git fetch and the git merge sequence.
		
		git pull origin

## git push

	Pushes all the modified local objects to the remote repository and advances its branches.

		git push origin master

## git remote add

	git remote add origin https://github.com/user/repo.git
	# Set a new remote

	git remote -v
	# Verify new remote
	origin  https://github.com/user/repo.git (fetch)
	origin  https://github.com/user/repo.git (push)


