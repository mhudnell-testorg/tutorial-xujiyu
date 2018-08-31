# Git tutorial 
Complete the steps below to learn about cloning, branching, committing, merging, and pushing in git! :octocat:

1. Clone this assignment to your desktop. Then cd into the directory. (Replace with your GitHub username)
```bash
  $ git clone ...
  $ cd tutorial-<username>
```
2. Create a file called 'last_meal.md'. Go to the Wikipedia page of your favorite food, and copy the first paragraph into it. Use Vim or your favorite text editor.
```bash
  $ vim last_meal.md
```
3. Use "git add" to stage your file. Then use "git commit" to commit all your staged changes.
  * Tip: use "git status" and "git log" to see confirmation of the changes you're making
  * Tip: use "-m" to give a description to your commit
```bash
(optional) $ git status
           $ git add last_meal.md
(optional) $ git status
           $ git commit -m "adding my favorite food"
(optional) $ git log
```
4. Create a new branch and switch to it.
  * Tip: use "git branch" with no argument to see all the branches
```bash
(optional) $ git branch
           $ git branch feature-drink
(optional) $ git branch
           $ git checkout feature-drink
```
5. Go to the Wikipedia page of your favorite drink, copy the first paragraph and append it to last_meal.md. Then stage and commit.
```bash
(optional) $ git status
           $ vim last_meal.md
           $ git add last_meal.md
(optional) $ git status
           $ git commit -m "adding my favorite drink"
```
6. Switch back to 'master' branch, read the contents of last_meal.md. Does it have both your meal and drink?
```bash
  $ git checkout master
  $ cat last_meal.md
```
7. Merge your drink branch into master. Now what does last_meal.md look like?
```bash
  $ git merge feature-drink
  $ cat last_meal.md
```
8. Push your changes to GitHub
```bash
  $ git push origin master
```
9. Go back to your repo on GitHub and refresh to see the changes you made!
