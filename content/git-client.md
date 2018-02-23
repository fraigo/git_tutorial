
## Git client 


### Download a Git client

After we get and confirm the GitHub account, we need to install a **Git Client** to access your code locally, in your computer. The Git client can be **downloaded** from https://Git-scm.com/downloads (Git Downloads):

1. [Git for **Windows**](https://git-scm.com/download/win) - https://git-scm.com/download/win
2. [Git for **Mac**](https://git-scm.com/download/mac) - https://git-scm.com/download/mac
3. [Git for **Linux**](https://git-scm.com/download/linux) - https://git-scm.com/download/linux

### Install your Git client 

The *instalation* process of Git Client is simple. You may be prompted to choose a few options while installing the client.

Once the installation is completed. You can **test the `Git` command** in a terminal/command window:

```bash
git --version 
```

The result will appear with a text like this:

```
Git version 2.14.3 (Apple Git-98)
```   
   
If there were any error messages like the following, you need to check your instalation process:
    
```
Git: command not found
```
    
### Configure your Git client

After you installed your Git client, you need to put some information about the Git user account in a terminal/command window. 

* First, define the **user name** of your Git account:

```bash
git config set user.name "My Name"
```

* Then, define the **user email** of the Git account:

```bash
git config set user.email "my.email@host.com" 
```











