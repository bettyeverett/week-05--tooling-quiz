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
