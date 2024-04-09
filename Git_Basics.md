# Git basics

- #### Setup Git

  - Install git
  - Configure name, email for commits
    ```sh
     git config --global user.name "Your name"
     git config --global user.email name@example.com
    ```
  - Create ssh keys using the `ssh-keygen` command
  - Add the public key to you Github account

- #### Intialize a empty git repository

  ```sh
  git init
  ```

- #### Add files to track

  ```sh
  git add <file_name> # add a single file
  git add <folder_name> # add a folder
  git add . # add everything under current directory
  ```

- #### Commiting changes

  ```sh
  git commit -m "Commit message"
  ```

- #### Ignoring files

  - Create a `.gitignore` file and add files/folders or [patterns](https://git-scm.com/docs/gitignore#_pattern_format) to exclude
  - Example
    ```sh
     echo .env > .gitignore
    ```

- #### Branches
  ```sh
  git branch # list all local branches
  git branch -a # list local and remote branches
  git checkout <branch_name> # checkout existing branch
  git checkout -b <branch_name> # create a new branch and checkout
  ```
- #### Common ways to integrate changes between different branches

  - Merge [(read more)](https://git-scm.com/docs/git-merge)

    ```sh
        git checkout <base_branch>
        git merge <other_branch>
    ```

  - Rebase [(read more)](https://git-scm.com/docs/git-rebase)

- #### Clone an existing remote repository

  ```sh
   git clone <repo_url>
  ```

- #### Configure a remote repository in an existing local git repository

  ```sh
   git remote add <remote_name> <remote_url>
  ```

- #### Pull changes from a remote repository

  ```sh
   git pull <remote_name> <branch_name> # push to a specific branch
  ```

- #### Push changes from a remote repository

  ```sh
   git push <remote_name> <branch_name>
  ```

- #### Stash changes

  ```sh
  git stash # stash all local changes
  git stash pop # restore stashed content (might cause conflicts)
  ```
