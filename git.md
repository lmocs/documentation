## Generating new ssh key for git
1. ```ssh-keygen -t rsa -C "loganmoreno.cs@gmail.com"```
2. Press enter for everything
3. ```cat ~/.ssh/id_rsa.pub```
4. Copy everything
5. Go to GitHub SSH settings
6. Add a new key and paste
7. If password auth continues to show, ```git remote set-url origin git@github.com:username/repo.git```

## Set git's default editor to vim
```git config --global core.editor "vim"```

## Merge a branch into `main`.
```
git switch main
git pull origin main
git merge <branch_name>
git push origin main
```

## Rebase when local main is behind remote main (branch divergence).
```
git fetch origin
git rebase origin/main
git push origin main --force-with-lease
```
NOTE: `--force-with-lease` prevents overwriting any new changes added by someone else.
