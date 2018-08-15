## Git Commands

### Tipycal workflow

When you are working with a Git project, you probably will use the following sequence of commands.

Remember that all command are executed from the root folder of your project.


#### Start a completely new project 

* `git init` to **start a new project** from scratch. It will create the basic Git **local** repository.

#### Start from a remote repository (clone)

* `git clone https://github.com/user/github-project.git` to start from a **local copy** of some existing project

* If you want to make changes to an existing repository *of another user*, you need to [**Fork** it] before cloning(content/github-projects.md#fork-a-github-project)

#### Use existing code or create files for a new git repository

* `git init` if the local repository was not initialized yet
* Create and modify any file inside the repository
* `git add -A` to add all files to commit
* `git commit -m "Initial commit"` to commit your changes **locally**.
* `git remote add origin https://github.com/user/project-name.git` to register a **remote** existing repository
* `git push -u origin master` to send your changes to the remote git repository.



#### Work with your project

* `git pull` to update your repository to the last changes

* `git status` to check if there is any new or modified file to commit or push.

* `git add path/to/file` to add a **new or modified** file to the index (to be commited) 

    * `git add -A` is a shortcut to add **all new and modified** files.

    * Also you can use wildcards (`git add path/to/*.js`) or multiple files separated by space (`git add path1/file.js path2/file2.js`)

* `git commit -m "Commit message"` to commit your changes from the index. 

* `git push` to upload your changes to GitHub.


#### Work with repositories and branches

* `git branch`
