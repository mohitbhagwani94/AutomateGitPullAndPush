# AutomateGitPullAndPush
To make git operation function automatic just add script.sh file in your project.

>Make this file executable, by running below command.
```
chmod 755 script.sh
```
Write the below command inside your terminal.
```
sudo git config --global credential.helper store
```
To run the executable file type the below command
```
./script.sh
```

Enter your usename and password.

Just you have to enter your password once, Afterwards you have to just run the script no need to type username and password again.

### Change commit message
> 1. Either Change the msg in script.sh file every time you commit.
> 2. Or assign some variable for commit msg, overwrite whenever you run this script and replace this varible with the commit msg in script.sh  (wait till my next commit, to reflect this change).

### ATTENTION
**Your username and password will be saved in plain text format inside ~/.git-credentials file.**

To reset or change you ~/.git-credentials file use below two commands.
```
git config --global --unset credential.helper
git config --system --unset credential.helper
```

**Note**
It you don't want to commit script.sh file. We have two solution
>1. Add script.sh in .gitignore file.
>2. Add this line ```git reset script.sh``` after line 8 in script.sh file.

!!!Happy Coding!!!
