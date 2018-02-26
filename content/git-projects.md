Z   
## Working with a Git project

GitHub allows you to modify and update your files directly on the GitHub website. But if you want a **better control** over your whole project, you can **work locally**, in your computer, in a Git project. These are the typical commands you need to work in a Git repository using the [Git client](git-client.md): 
   
### Clone a Git project

Using the [command line Git client](git-client.md) you can download a copy of your repository using the GitHub project url. Typically the clone URL follows this format:

```
https://github.com/your-user/your-project.git 
```

You can get the git project URL using the green button labeled "Clone or download"

![GitHub Project Page](../images/github-project.png)

The link shown is your Git clone URL. Copy this URL and execute the **clone** command:

```
~> git clone  https://github.com/your-user/your-project.git 
cd your-project/
```

The first command will download a copy (clone) of your repository and will **create a folder** with the same name of your folder. The second step is to enter to the newly created folder. 


### Pull external changes

Once you have cloned the project, and before you start a new group of changes, you may need to **pull** the remote repository (retrieving new changes made externally), to make sure you have the last version of the files.

```
git pull
```



### Status of your project

You can **check the status**s of your files (ok, modified, added, removed) using the status command:

```
git status
```


### Add files to your project

Now you can do whatever file operation in your project folder created: create new files, move files from another directory, and remove files not used. 

```
git add path/to/file.ext
git rm path/to/deleted/file.exe
```


### Commit your changes

Before you commit your files, you need to check the status of your files, and if something has not been added (files in red). If everything looks ok, then you can commit your changes using the **commit** command:

```
git commit -m "Message to be recorded in your transaction".




### Submit changes to rour GitHub

Where you feel you are redy with your files and new features, 
you may "push" your project to merge with the main repository.

```
git push
```

 





































































































### Push your commits to GitHub




