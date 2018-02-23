
## Git Client 


### Download a Git client

After we get and confirm the GitHub account, we need to install a **Git Client** to access your code locally, in your computer. The Git client can be **downloaded** from https://Git-scm.com/downloads (Git Downloads):

1. [Git for **Windows**](https://git-scm.com/download/win) - https://git-scm.com/download/win
2. [Git for **Mac**](https://git-scm.com/download/mac) - https://git-scm.com/download/mac
3. [Git for **Linux**](https://git-scm.com/download/linux) - https://git-scm.com/download/linux

### Install your Git client 

The *instalation* process of Git Client is simple. Follow all the instructions of the installation process. You may be prompted to choose a few options while installing the client.

### Accessing the terminal window

If you are using Windows, Linux, or Mac, you may have different ways to access a terminal/command window. This terminal allows you to execute git commands:

* For Linux (Ubuntu, Debian, etc), you can use the default **Terminal** application.
* For Windows you can use the **Git shell** terminal, *installed along with the Git client*
* For Mac, use the **Terminal** application located in *Apps/Accessories*

### Testing your Git client installation

Once the installation is completed. You can **test the `Git` command** in a [terminal/command window](#accessing-the-terminal-window):

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

After you installed your Git client, you need to put some information about the Git user account in a [terminal/command window](#accessing-the-terminal-window). 

* First, define the **user name** of your Git account:

```bash
git config set user.name "My Name"
```

* Then, define the **user email** of the Git account:

```bash
git config set user.email "my.email@host.com" 
```


### Getting the SSH key for GitHub access

If you plan to push your changes to a GitHub account, you need to share a SSH key to access the GitHub server.

Open a [terminal/command window](#accessing-the-terminal-window) and check if you have a public SSH key created (`id_rsa.pub` stored in a hidden folder `.ssh/` in your home folder):

```bash
cat .ssh/id_rsa.pub
```

The result is the content of the id_rsa.pub file, which looks like the following example. Copy the contents to the clipboard.

```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCfKooeX2AxyQVdBrvFZCIOGRJ279zGc8qY6kHXhzK9i+fllfDGe/ceyfW9vGXf8rwesE963/wuWut842OGZDmbyPtqajDl7lETiWKHBWK/3FLaQsien31fbT8mV5mTIUkWGMJMYT0EjBtusovLWr5Tjvpn8TdAHt9SLFLPA6RcgLSIta8fzib5/WPu2UOsf5BBRP6eQquoehLsk5cxyWnha06fuRKNrzSLTSMdfFeigHEuzNAOraJvq/E/NGrAX1mE/Dfi8qpnhwOpPY308rxwuVrfp6whBrEvchF/zbWzXXXVbjL1dMc4tiX/itGGt2QBf1lA5Tm9D/oBo5lJr7vl admin@admins-MacBook-3.local
```

If you get a "`not such file or directory`" error, you need to [create a public SSH key](#creating-a-new-public-ssh-key):


#### Creating a new public SSH key

Open the terminal in your home directory and execute the `ssh-keygen` command (generate a SSH public/private key pair)

```bash
ssh-keygen
```

You will be prompted to **set a filename** to store the key and **set a passphrase** two times. You can *leave blank* this values (press [Enter] and continue) to use the default values. The result is a randomart image and 2 files: `.ssh/id_rsa` and `.ssh/id_rsa.pub` (the last one is your public key)

```
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/admin/.ssh/id_rsa):               
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /Users/admin/.ssh/id_rsa.
Your public key has been saved in /Users/admin/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:y7g4UqntpnFzLsA8BpsSlx/Yr01FcU1KsiNDQ0k8uJw admin@admins-MacBook-3.local
The key's randomart image is:
+---[RSA 2048]----+
|     ==.o.oo.    |
|    ..+..= ..    |
|   = oooo .      |
|o + E  o..       |
| O . + .S        |
|+ * + oo .       |
|...*o+o o        |
|  oo*=..         |
|  .=ooo          |
+----[SHA256]-----+
```

Once you have created your SSH keys, now you can [get the public SSH key](#getting-the-ssh-key-for-github-access).














