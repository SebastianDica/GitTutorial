# GitTutorial

## What is Git?
Git is a free and open source distributed version control system designed to handle everything from small to very large projects.
- https://en.wikipedia.org/wiki/Git

## Why Git?
Your project may go through many stages of development. Git provides a way to track its history and control the versions at each time step.

## Git vs. GitHub
Git is the mechanism by which version control happens. GitHub is a UI built on top of Git.
- https://git-scm.com/

## GitHub vs. Alternatives
GitHub is not the only UI built on top of Git. There are some alternatives:
- https://about.gitlab.com/
- https://bitbucket.org/

## Examples in the real world
Git is used in the real world in many areas:
- https://github.com/CSSEGISandData/COVID-19
- https://github.com/mrc-ide/covid-sim
- https://github.com/Mojang
- https://github.com/EbookFoundation/free-programming-books

## Installing Git
Installing Git depends on your machine:
https://github.com/git-guides/install-git

Credentials may be required.

## Git on paper
![Github drawio](https://user-images.githubusercontent.com/10688697/134654690-e1841c2d-2802-4c3c-9778-f6e0a1b8bdea.png)

## Terminology
- repository - a collection of files which represnt your project
- main branch - the current version of the project
- active branch - a version of your project which is diverged from the current main branch by some changes
- merged branch - an inactive branch which used to be active and has been united with the main branch
- commit - a change to the project which is identified by a hash code
- origin - the git server configuration on your local machine
- merge - the action of combining two branches
- fork - snapshotting a repository into another repository for developing parallel work

## Commands

### Git Help
Used to get help with git.
```bash
git --help
```

Used to get the git manual.
```bash
man git
```

### Git Init
Used to create a local repository on your machine.
```bash
git init
```

### Git Clone
Used to copy a repository onto your machine.
```bash
git clone https://github.com/SebastianDica/GitTutorial.git
```

### Git Pull
Used to pull the latest version of a branch onto your machine
```bash
git pull origin main
```

### Git Checkout
Used to create a new branch
```bash
git checkout -b new_branch_name
```

Used to get the last tracked version of a file
```bash
git checkout filename.json
```

### Git Status
What is the current status of your local repository?
```bash
git status
```

### Git Diff
What is the difference between original starting commit and the changes you have made?
```bash
git diff
```

### Git Add
Used to tell git that you are interested to track certain files.
```bash
git add filename.json
```

Used to tell git that you are interested to track all files.
```bash
git add -A
```

### Git Commit
Used to tell git that you want to create a commit with the tracked files.
```bash
git commit -m "name of your commit"
```

### Git Push
Used to tell git that you want to push your commit to a branch.
```bash
git push origin branch_name
```

## UIs and practices

### Pull Requests
In the pull requests tab on this repository, you can create pull request out of one of your branches.

This tells everyone that you want to merge your branch into the main branch.

### Reviews
People can then review your branch to see whether or not it would be valid to merge.

### Merging
The pull request will have a button called 'Merge' which will perform the merge action and will close your pull request if succesful.

### Conflicts
If both branches modify the same file lines, there may be some conflicts. Consequentially, these need to be resolved by the user manually in most cases.

## Visualizers

A way to visualize the git tree graph.
```bash
git log --graph --decorate --oneline
```

## In the industry
- used every day for producing code
- used for tracking state of software over time
- latest code breaks production? git allows us to revert to a previous working version
