[回到目录](../../README.md)

<hr>
<hr>
<br>

# | Git |

## [00:10:30] Why git

### Version Control

## [00:16:30] Centralized and Distributed

Centralized - Subversion:
one code base one repos

Distributed - Git:
local and remote

## [00:27:00] Git and GitHub

## [00:33:30] Set up version control

### Set up Git config

- Setup user name: `git config --global user.name "<Your-Full-Name>"`
- Setup user email: `git config --global user.email "<Your-Email-Address>"`
- Setup UI Color: `git config --global color.ui.auto`
- Setup merge conflict style: `git config --global merge.conflictstyle diff3`
- Setup editor: `git config --global code.editor "code --wait"`
- Check Config: `git config --global --list`

### Set up Git Repository

Two ways to create a new repository:

1. `git init`
2. `git clone <remote URL>`

DON'T TOUCH `git` FOLDER AFTER THIS

## [00:50:00] Commit Changes

### Add files to stage:

- Stage Selected: `git add <file path>`
- Stage All: `git add *`

### Stage:

- Check Status: `git status`

  ```
  $ git status
  On branch lectures/05-git
  Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
      new file:   course-materials/05_git/Git-Assignment.docx
      new file:   course-materials/05_git/Git-Quizes.docx
      new file:   course-materials/05_git/Github-CheatSheet.pdf
      new file:   course-materials/05_git/IntroToGit.pdf
  ```

- Unstage changes: `git restore --staged <file>`

### Commit Changes: `git commit`

### [01:12:00] Commit Message - IMPORTANT

### Undo Commit

### [01:27:30] Git status and history

_[00:29:00 - Class Break]_

## [01:42:00] Branch

### Merge

### Git Graph

## [00:00:00] Pull Request

## [00:00:00] Resolving Conflict

## [00:00:00] Merge vs Rebase
