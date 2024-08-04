# Generating new ssh key for git
ssh-keygen -t rsa -C "loganmoreno.cs@gmail.com"
Press enter for everything
cat ~/.ssh/id_rsa.pub
Copy everything
Go to GitHub SSH settings
Add a new key and paste
If password auth continues to show, git remote set-url origin git@github.com:username/repo.git

# Set git's default editor to vim
git config --global core.editor "vim"
