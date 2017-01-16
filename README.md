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
It ask for user name and password. Enter your usename and password.

Just you have to enter your password once, After that it work automatically.

ATTENTION
Your username and password will be saved in plain text format inside ~/.git-credentials file.

To reset or change you ~/.git-credentials file use below two commands.
```
git config --global --unset credential.helper
git config --system --unset credential.helper
```

