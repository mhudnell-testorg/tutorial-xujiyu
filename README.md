# Git tutorial 
Complete the steps below to learn about cloning, branching, committing, merging, and pushing in git! :octocat:

1. Clone this assignment to your desktop. Then cd into the directory. (Replace with your GitHub username)
```bash
  $ git clone https://github.com/mhudnell-testorg/tutorial-<username>.git
  $ cd tutorial-<username>
```
2. Create a file called 'last_meal.md'. Go to the Wikipedia page of your favorite food, and copy the first paragraph into it.
```bash
  $ vim last_meal.md
```
3. Stage your file, then commit it to the master branch.
```bash
  $ git add last_meal.md
  $ git commit -m "adding my favorite food"
```
4. Create a new branch and switch to it.
```bash
  $ git branch feature-drink
  $ git checkout feature-drink
```
5. Go to the Wikipedia page of your favorite drink, copy the first paragraph and append it to last_meal.md. Then stage and commit.
```bash
  $ git add last_meal.md
  $ git commit -m "adding my favorite drink"
```
6. Switch back to master branch, read the contents of last_meal.md. Does it have both your meal and drink?
```bash
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
9. (Optional) Observe your commits
```bash
  $ git log
```
