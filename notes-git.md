# Git Notes ![Git badge](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)

This section contains common uses for Git These common uses are useful for all the repositories. 

## How to Get a Remote Repository on GitHub to Your Local Machine
Steps: 
1. Go to GitHub. 
2. Click into the target remote repository. 
3. Click the [Code] button. 
4. Select the [HTTPS] tab. 
5. Copy the HTTPS URL. 
6. Open a command-line interface (CLI). 
7. Use the `cd` command followed by the directory path to change the directory to the one you want to put the entire remote repository in[^1]. 
8. Type `git clone` followed by the HTTPS URL copied to clone a copy of the remote repository[^2]. 
9. Press [ENTER]. 
[^1]: 
    A folder with the same name and structure as the remote repository will appear in the exact directory in which the `git clone` command is used on your local machine. 
[^2]: 
    It is unnecessary to use `git init` before `git clone`. The cloned respository already has `.git` folder inside it. 

## How to Create a New Repository
Steps: 
1. Go to your profile page on GitHub. 
2. Select the [Repositories] tab. 
3. Click the [New] button. 
4. Name the new repository under "Repository name". 
5. Choose whether the repository should be [Public] or [Private]. 
6. Click the [Create repository] button[^3]. 
7. Open a command-line interface (CLI). 
8. Use the `cd` command followed by the directory path to navigate to the desired directory on your local machine[^4]. 
9. Use the `mkdir` command followed by the name of the remote repository to create the corresponding local repository. 
10. Use the `cd` command followed by the folder name to go inside it. 
12. Type `git init` to let Git start tracking the local repository. 
13. Type `git add .` to add all the files inside the local repository to the staging area[^5]. 
14. Type `git commit -m "commit message"` to capture a snapshot of the currently staged changes in the repository[^6]. 
15. Type `git branch -M main` to forcefully rename the default branch to "main"[^7]. 
16. Click into the remote repository.
17. Click the [Code] button. 
18. Select the [HTTPS] tab. 
19. Copy the HTTPS URL. 
20. Type `git remote add origin` followed by the HTTPS URL to add the remote repository's reference to the local repository[^8]. 
21. Type `git push -u origin main` to push the code from your local to the `main` branch of the remote repository at the HTTPS URL referenced by `origin`[^9]. 

[^3]: 
    You can also choose whether you want to add `README.md`, `.gitignore` and `LICENSE` filles to the newly created repository before clicking the [Create repository] button. 
[^4]: 
    You can also use the file manager application in your system to do this. 
[^5]: 
    This will direct Git to save a snapshot of the current project state into the commit history. 
[^6]: 
    This will tell Git to keep track of the progress and changes of the project so that you can recall or revert to the committed changes at a later date. 
[^7]:
    If you create a remote repository without adding a file (including `README.md`, `.gitignore` and `LICENSE`) inside, there will not be any branch yet. Once you add one or more files to the remote repository, the default branch will be `main` on GitHub. But when you `git add` files in the corresponding local repository, the default branch will be `master`. Therefore, you need to use `git branch -M main` to rename the local branch from `master` to `main` to match the remote repository branch setting. 
[^8]:
    `origin` references the HTTPS URL to the remote repository to push to from/pull from to the local repository. 
[^9]: 
    The `-u` options is a shorthand for `--set-upstream` which is used to map a local branch to a remote barnch. 

## Extra: How to Set Up a Local Branch to Track a Remote Branch
### Case 01
<ins>Background</ins>: You are currently on the `main` branch and have added a remote reference `origin`. 
<br />
<ins>Full Command</ins>: ```git branch --set-upstream-to=origin/main main```
<br />
<ins>Short Command</ins>: ```git branch -u origin/main main```

### Case 02
<ins>Background</ins>: You are not currently on the `main` branch and have added a remote reference `origin`. 
<br />
<ins>Full Command</ins>: ```git branch --set-upstream-to=origin/main```
<br />
<ins>Short Command</ins>: ```git branch -u origin/main```

## Error: `failed to push some refs to 'https://github.com/....git'`
<ins>Cause</ins>: The remote repository contains work that you do not have locally. 
<br />
<ins>Fix</ins>: Integrate the remote changes using the following command:
```
git pull origin main
```

## Error: `refusing to merge unrelated histories`
<ins>Cause</ins>: Two respositories have mismatching histories and are considered unrelated. 
<br />
<ins>Fix</ins>: Add the following option to allow unrelated histories to be merged:
```
git pull origin main --allow-unrelated-histories
```
