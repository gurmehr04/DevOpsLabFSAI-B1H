Lab 5:

# *Git Submodules*

## *Git Workflow for Multiple Repositories and Submodules*

This session involves:

- Cloning multiple repositories
- Creating files
- Adding and committing changes
- Setting up Git submodules
- Pushing updates to remote repositories

---

## *Step 1: Cloning Repositories*

You cloned three repositories from GitHub:

```sh
git clone https://github.com/jahnaviichauhan/DemoMain.git
git clone https://github.com/jahnaviichauhan/DemoCSS.git
git clone https://github.com/jahnaviichauhan/DemoJS.git
```

💡 Note: There was an error (gir clone instead of git clone).

---

## *Step 2: Creating Files in Each Repository*

### In DemoJS repository:
```sh
cd DemoJS
touch script.js
```

### In DemoCSS repository:
```sh
cd ../DemoCSS
touch style.css
```

### In DemoMain repository:
```sh
cd ../DemoMain
touch index.html
```

---

## *Step 3: Committing and Pushing Changes*

For each repository, you added, committed, and pushed the files.

### For DemoMain
Earliest to latest commits:
```sh
git add .
# 1st commit
git commit -m "Added basic website HTML file"
# 2nd commit
git commit -m "this is a commit"
# 3rd commit
git commit -m "Path added"
# 4th commit
git commit -m "Merge branch 'main' of https://github.com/jahnaviichauhan/DemoMain"
# 5th commit
git commit -m "made a change in index.html style.css"
# 6th commit
git commit -m "css folder deleted"
# 7th commit
git commit -m "Added CSS folder"
# 8th commit
git commit -m "sync"

git push
```

### For DemoJS
Earliest to latest commits:
```sh
git add .
# 1st commit
git commit -m "Added script.js"
# 2nd commit
git commit -m "Js"
# 3rd commit
git commit -m "js configured"

git push
```

### For DemoCSS
Earliest to latest commits:
```sh
git add .
# 1st commit
git commit -m "css file"
# 2nd commit
git commit -m "folder"
# 3rd commit
git commit -m "CSS"
# 4th commit
git commit -m "css changed backgroundcolor"

git push
```

---

## *Step 4: Setting Up Git Submodules*

You added DemoCSS and DemoJS as submodules inside DemoMain:

```sh
git submodule add git@github.com:jahnaviichauhan/DemoCSS.git css
git submodule add git@github.com:jahnaviichauhan/DemoJS.git js
```

Then, you committed and pushed the changes:

```sh
git commit -m "added css to main"
git push
```

```sh
git commit -m "added js to main"
git push
```

---

## *Step 5: Verifying Repository Status*

Checking the status:

```sh
git status
```

---

## *Explanation of the Workflow*

This document demonstrates a structured approach to managing multiple repositories with Git submodules. The key steps include:

1. *Cloning Repositories:* Downloading code from remote repositories to the local environment.
2. *File Creation:* Establishing required files (index.html, style.css, script.js) in respective repositories.
3. *Commit Management:* Accurate and sequential commit messages reflect project history transparently.
4. *Submodule Integration:* Adding external repositories (DemoCSS, DemoJS) as submodules in DemoMain for modular project management.
5. *Verification of Status:* Using git status to ensure the working directory is clean and ready for future development.

