Hell Nava!

##look at the commits of the current branch, newest at top
git log

##look at all remote branches with local branches
git branch -a

##Show parental replationships as well
git log --graph --oneline

##Show parental relationships starting from the given branch name
git log --graph --oneline origin/development


GIT Tags:
( a human redable label for a particular commit)
    ##tags must be unqiquely quoted
     Non-annotated tags:
       git tag v1.0
     Annotated tags:
      git tag -a beta7 -m "this is the beta7 version..."



GIT Branches:
(A git branch is a git tag that can move)( a branch is pointer to a commit that can move  based on acctions you take)
deleteing the barnch doesn't delete all the commits, it's jut delets the specific pointer 

##observe current branch
git branch

##create new branch
git checkout -b development

##commit
git add <filename>
git commit -m "this is the"

##observe the location of your new branch in the tree
git log --online --graph -all --decorate

##delte your branch
git branch -d <branchname>
##Force delete branch
git branch -D <branchname>

##restore branch
git checkout -b <branchname> <commit sha1>

##where in the tree the branch is created is important. It will be created
##at HEAD unless otherwise specified
git checkout -b <branchname> <REF>
REF-> is a commit, tag, local branch, remote branch, or any other specification of a point in history