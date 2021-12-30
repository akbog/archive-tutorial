# GitHub Archive Tutorial

## Introduction

Git and GitHub are tools that help developers of all walks of life monitor changes in the code that they write over time. Git is very simply put a system that comes pre-installed in most operating systems and once initialized in a given directory, takes notes and monitors the changes made to files in that directory. This is controlled via a series of operations that add and commit changes to a living code tree. The reason that your code can take the form of a tree is due to the existence of branches, which are an opportunity to have multiple **versions** of your code existing at the same time. For instance, if you've ever been asked to make a change to a piece of code that might take you a few days to complete, but then been asked to change another part of your code that might take you an hour, you could create a new **branch** which would allow you to commit the second change while maintaining your progress towards the longer goal in a separate branch.

GitHub (not the same thing as Git) is a web-application and repository cloud-storage solution. It provides a place for you to upload your code (i.e. repository) which means you don't have to worry about losing any of your code in the case of a hardware failure. This is done by adding, commiting (Note: adding and commiting are Git commands), and most-importantly pushing (Note: this is where GitHub comes in) your code to a repository that you initialize in GitHub.

### Heads Up!!!

1. GitHub is not meant to archive large files (e.g. data files, csv's, .gz's etc.) - these should be specifically ignored in a .gitignore file
2. Make sure to split up your repositories intelligently (i.e. if your code is composed of multiple scripts that each do something else with different inputs and are unrelated, consider putting them in different repositories)

### Standard Git Commands

```
init: initializes a repository

add: adds current changes made to a given file (or all files with ".") to the current commit

commit -m "{your commit message}": commits changes made to the files mentioned in add

push: pushes changes made to a remote repository (e.g. GitHub)
```

## How To: Create a new Repository in GitHub

1. New **GitHub** Repository

Navigate to your github (or your organizations if you have one) and click new:

![New Repo](https://github.com/akbog/archive-tutorial/blob/main/images/new-repository.png)

2. Create the Repository

Make sure to select the appropriate level of visibility. If you're part of an organization, you might want to maintain a certain level of privacy:

![Create New Repo](https://github.com/akbog/archive-tutorial/blob/main/images/create-new-repository.png)

3. Follow New Repo Directions

![New Repo Tips](https://github.com/akbog/archive-tutorial/blob/main/images/follow-new-repo-directions.png)

## How To: Add, Commit, and Push Changes

1. Initialize a Local Repository using the following command:

```
git init
```

2. If you already have existing files, add them to your repository with this command:

```
git add .
```

You may optionally also add files / changes individually as follows if you'd only like to commit changes made to certain files:

```
git add filename.txt filename2.txt
```

3. Commit your changes

Git considers a commit to be a specific version of your code that you'd like to keep. In this way, you may revisit previous "commits" to find previous versions of your code. Think of commits as breakpoints in the timeline of your code that you can visit. When you make a major change to your code, consider creating a unique commit just for that change and providing a brief but explanatory commit message alongside it. 

```
git commit -m "feature: {description of the change you're commiting}"
```

4. Push your changes

Finally, git push pushes your change to a remote repository such as GitHub.

```
git push
```

## Help

Always appreciated.

## Authors

Contributors names and contact info

> Alexander Bogdanowicz [@akbog](https://github.com/akbog)
