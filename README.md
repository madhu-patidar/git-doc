## Install Git

	sudo apt-get install git

## git config

Sets configuration values for your user name, email, gpg key, preferred diff algorithm, file formats and more.

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
	
	## git remote add

	git remote add origin https://github.com/user/repo.git
	# Set a new remote

	git remote -v
	# Verify new remote
	origin  https://github.com/user/repo.git (fetch)
	origin  https://github.com/user/repo.git (push)


## git commit

Takes all of the changes written in the index, creates a new commit object pointing to it and sets the branch to point to that new commit. 

	git commit -m ‘committing added changes’

## git checkout

Checks out a different branch – switches branches by updating the index, working tree, and HEAD to reflect the chosen branch.
		
	git checkout newbranch

## git branch

1. List all of the branches in your repository.

		git branch 

2. Create a new branch called branch_name. This does not check out the new branch.

		git branch branch_name
		
3. Delete the specified branch. This is a “safe” operation in that Git prevents you from deleting the branch if it has unmerged changes.
	
		git branch -d branch_name
		
3. Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.

		git branch -D branch_name

4. Rename the current branch to branch .

		git branch -m branch_name

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

