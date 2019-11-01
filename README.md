# Quiz
---
## 1. Getting setup with Git

`git remote add origin git@github.com:develop-me/drupal1.git`

The above command sets the github repository's origin to the local master file that you have created on your computer. After you have initialised to work with git on your system, you can then create a repository in your github account and allow others to contribute to the same project if you share the repository with them.

## 2. Committing Files

```bash
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   hello.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	images/
	index.html
```
In order to commit the images folder and index.html, I would use the commands...

```bash
git add images/ index.html
git commit -m "Apple"
```

Then to save hello.html in the next commit...

```bash
git add hello.html
git commit -m "Banana"
```
Alternatively, I could use...

`git commit -am "Banana"`

## 3. Reading Git Messages: Oh Noes #1

```bash
To github.com:develop-me/git-simple.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:develop-me/git-simple.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

The above message has been returned when trying to push a version to the repository.

The error message is telling us that we can't push to the repository because your version is older than the current version in the repository and therefor you would overwrite and lose work in the repo. You would need to pull the current repo first to merge with your local work before pushing and updating the repo.

