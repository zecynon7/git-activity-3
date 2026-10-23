# Git Activity 3 — Commands and Procedure

Replace `YOUR-USERNAME` with your GitHub username if needed.

## 1. Clone the repository
```bash
git clone https://github.com/zecynon7/git-activity-3.git
cd git-activity-3
```

## 2. Create and commit the sample file
The repository includes `git-activity.txt`. If completing this step from scratch, create it with a text editor, then run:
```bash
git status
git add git-activity.txt
git commit -m "Initial commit"
git push origin main
```

## 3. Create and switch to a feature branch
```bash
git checkout -b feature-branch
```
Edit `git-activity.txt` and add a line such as `Update made on feature-branch.` Then run:
```bash
git add git-activity.txt
git commit -m "Update activity text on feature branch"
git push -u origin feature-branch
```

## 4. Merge the feature branch into main
```bash
git checkout main
git pull origin main
git merge feature-branch
git push origin main
```
If GitHub reports the branches have diverged or the feature branch is not pushed, resolve that state before continuing. A pull request is an alternative way to merge on GitHub.

## 5. Make a change on GitHub and pull it locally
On GitHub, open `git-activity.txt`, choose Edit, add a line such as `Update made directly on GitHub.`, and commit the change to `main`. Then, in your local terminal:
```bash
git checkout main
git pull origin main
```

## 6. Verify and document
```bash
git status
git log --oneline --graph --all
```
Capture screenshots of your own terminal and GitHub repository if required by your instructor. The commands above are documentation; commands run through the GitHub website/API are not the same as running them in your local terminal.