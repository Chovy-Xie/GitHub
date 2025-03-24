# GitHub
> README.md [Formatting](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).


## Content
[Git Setup](#Git-Getting-Started)

[GitHub Clone Repository](#Git-and-GitHub)

[Create and Upload Local Files](#If-Already-Have-Local-Files-to-Upload)

[Pull Request](#GitHub-Send-Pull-Request)

[Merge](#Git-Merge-Branch)

[Additional Instruction](#Addition)


## Git Getting Started

### Git Install
You can download [Git](https://git-scm.com/) for free. 

### Using Git with Command Line
Check if Git is properly installed: 
```
git --version
```
If Git is installed, it should show something like:
> git version 2.47.0.windows.2

### Configure Git
```
git config --global user.name "user-name"
git config --global user.email "example@gmail.com"
```
Change the user-name and e-mail address to your own.


## Git and GitHub

### Git Clone
Copy the url from the green 'Code' button.
```
git clone https://github.com/Chovy-Xie/GitHub.git
```

### Git Pull
Pull the latest version
```
git pull origin main
```

### Create a new Branch
```
git branch <branch-name>
```

### Switch to Another Branch
```
git checkout <branch-name>
```

### Adding Files
```
git add .
```

### Commit
```
git commit -m "Comment"
```

### Push the Branch to GitHub
```
git push origin <branch-name>
```

### GitHub Send Pull Request
[w3schools](https://www.w3schools.com/git/git_remote_send_pull_request.asp?remote=github)

### Git Merge Branch
```
git checkout <another-branch>
git pull origin <another-branch>
git checkout <your-branch>
git merge <another-branch>

# fix conflict
Press I  # enter "insert mode" to edit commit message manually
Press Esc  # exit "insert mode"
:wq  # write(save) the file and quit vim
:q!  # or quit without saving (if you want to cancel) 

git push origin <your-branch>
```

### Addition
```
mkdir <directory-name>  # make a new directory
cd <directory-name>  # change the current working directory
cd ..
cd ../..
ls  # list directory contents
pwd  # print working directory
touch <file-name.txt>  # create a new file.txt
open <file-name.txt>  # open the file
cat <file-name.txt>  # display the file content
rm <file-name.txt>  # remove file or directory
mv <file-name.txt> <new-file-name.txt>  # rename files or directory>
```


## If Already Have Local Files to Upload

### Create a new Repository
1. Go to [GitHub](https://github.com/) and log in to your account.
2. Click the **New** button (+ icon).
3. Fill in the repository details: <ins>repo-name</ins>, <ins>description(optional)</ins>, <ins>Public</ins> or <ins>Private</ins>.
4. Do **NOT** initialize the repository with a <ins>README.md</ins>.
5. Click **Create** repository.

### Prepare Local Project
1. Open a <ins>terminal</ins> or <ins>Git Bash</ins>.
2. Navigate to your local project directory:
```
cd /path/to/your/project
```
3. Initialize a Git reposiotry:
```
git init
```

### Link Local Repository to GitHub
```
git remote add origin https://github.com/Chovy-Xie/GitHub.git
```

### Stage and Commit Local Files
1. Add all files to the staging area:
```
git add -A
```
2. Commit the changes:
```
git commit -m "Initial commit"
```

### Push Local Repository to GitHub
```
git branch -M main
git push -u origin main
```
