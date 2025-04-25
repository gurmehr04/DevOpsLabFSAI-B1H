Lab 1:

# *Basic Linux and Git Commands*

## *Installing WSL and NixOS*

### *1. Install Ubuntu using WSL*
To install Ubuntu using Windows Subsystem for Linux (WSL), run the following command in PowerShell:

```sh
wsl --install -d Ubuntu
```

### *2. Install NixOS in Single-User Mode*
For a NixOS single-user installation, follow the official documentation for proper setup.

---

## *Using Git Bash*
Git Bash provides a Linux-like terminal experience on Windows, enabling the use of standard Linux commands.

### *Common Linux Commands in Git Bash*

- **ls** → Lists files and directories.
- **pwd** → Prints the current working directory.
- **cd Desktop** → Changes the directory to the Desktop.

---

## *Basic Git Commands*

### *1. Cloning a Repository*

To clone a Git repository, use:
```sh
git clone "https://github.com/yourrepository.git"
```

### *2. Checking Remote Repositories*
```sh
git remote -v
```

### *3. Viewing Branches*
```sh
git branch
```

### *4. Checking Commit History*
```sh
git log
```

### *5. Checking Repository Status*
```sh
git status
```

### *6. Viewing Differences Between Commits*
```sh
git diff
```

### *7. Adding and Committing Changes*
```sh
git add filename
```
```sh
git commit -m "Your commit message"
```

### *8. Configuring Git with Your Name*
```sh
git config --global user.name "jahnaviichauhan"
```

---

## *Creating Files and Directories*

To create files for different purposes:

```sh
touch home
```
```sh
touch office
```

These commands create empty files named `home` and `office` in the current directory.

This article provides fundamental steps for setting up WSL, using Git Bash, and performing essential Git operations.

