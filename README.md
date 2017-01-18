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
Will ask for your commit message. 
``` 
Enter you commit message : Message
```

Enter your username and password.

Just you have to enter your password once, Afterwards you have to just run the script no need to type username and password again.


### ATTENTION
**Your username and password will be saved in plain text format inside ~/.git-credentials file.**

To reset or change you ~/.git-credentials file use below two commands.
```
git config --global --unset credential.helper
git config --system --unset credential.helper
```

**Note**
If you don't want to commit script.sh file. We have two solution
>1. Add script.sh in .gitignore file.
>2. Uncomment ```git reset script.sh``` this line in script.sh file.

!!! Happy Coding !!!
