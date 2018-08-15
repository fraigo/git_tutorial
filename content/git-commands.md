## Git Commands

### Tipycal workflow

When you are working with a Git project, you probably will use the following sequence of commands.

Remember that all command are executed from the root folder of your project.


#### Start a project 

* `git init` to **start a new project** from scratch. It will create the basic Git **local** repository.

* `git clone https://github.com/user/github-project.git` to start from a **copy of some existing project**

* If you want to make changes to an existing repository of another user, you need to [**Fork** it] before cloning(content/github-projects.md#fork-a-github-project)

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
