# Generating new ssh key for git
1. ```ssh-keygen -t rsa -C "loganmoreno.cs@gmail.com"```
2. Press enter for everything
3. ```cat ~/.ssh/id_rsa.pub```
4. Copy everything
5. Go to GitHub SSH settings
6. Add a new key and paste
7. If password auth continues to show, ```git remote set-url origin git@github.com:username/repo.git```

# Set git's default editor to vim
```git config --global core.editor "vim"```
