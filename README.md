- [Version control with Git and GitHub](#version-control-with-git-and-github)
- [Git installation](#git-installation)
- [Creating a profile in GitHub](#creating-a-profile-in-github)
- [Check if Git is properly installed](#check-if-git-is-properly-installed)
- [A few helpful commands to know](#a-few-helpful-commands-to-know)
- [Configure your Git](#configure-your-git)


## Version control with Git and GitHub
Version control is a process that tracks changes made to any file or program to fix a bug or make continuous improvements. Version control is done locally with git with a local repository, while a remote repository is hosted online in GitHub, GitLab, or Bitbucket.
### Git installation
The installation of Git is fairly straightforward. Go to [Git](https://git-scm.com/downloads), then download and install the version suitable for your operating system.
### Creating a profile in GitHub
You can create a profile on GitHub, GitLab, or Bitbucket. GitHub is the most popular one. While GitHub is not open-source, GitLab and Bitbucket are. I prefer GitHub, but you are open to choosing any of them. Go to [GitHub](https://github.com/) and create an account.
### Check if Git is properly installed
If you are using Windows, you can search for Git Bash in the Windows Start menu, or alternatively, right-click on any folder of your choice and select 'Open Git Bash here' to open a Git Bash shell. Remember that opening Git Bash shell from a folder would consider that folder as the current directory.
After opening the Git shell, let's verify that Git is correctly installed by running a few lines of code.

```PowerShell-linenums
 $git --version
```
Running this command returns 'git version 2.44.0.windows.1' for me. Probably yours should be something similar, depending on the version and operating system on which you have installed Git.
### A few helpful commands to know
Now, considering that Git is correctly installed. The first command one should learn is how to get help when necessary. 

```PowerShell-linenums
$git help commit
```
Will return in detail help for the command commit. Optionally, one could get concise help in the shell window itself by typing.

```PowerShell-linenums
$git commit -h
```
If you want to print your current working directory. You can write this command to print working directory.
```PowerShell-linenums
$pwd
```
To view existing files in the working directory, you can go ahead and execute the first command to list the files in your current directory. Optionally, you can add an alias to see all files, including hidden files.
```PowerShell-linenums
$ls
$ ls -laF
```
To change the current directory, see the commands below.
```PowerShell-linenums
$cd <PATH TO DESTINATION FOLDER>
$cd .. #will move backward one step to the previous folder
$cd #will take you to the home directory
$cd <FOLDER> #folder then shown in the list directory command, will take you to that directory
```
### Configure your Git
Probably, if you are a first-time user, you have not yet configured Git.
Running this command would show your name if you have already done so.
```Powershell-linenums
$git config user.name
```
If it does not display your name, you can set your user name and email address by running these commands in Git shell. Use the email address that you used to create your GitHub account.
```PowerShell-linenums
$git config --global user.name "YOUR NAME"
$git config --global user.email "YOUR EMAIL"
```
