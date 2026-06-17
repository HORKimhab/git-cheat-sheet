# Git Cheat Sheet

A personal Git cheat sheet containing the most commonly used commands, along with additional useful ones. 

Feel free to contribute and add more improvements.


## Branching 

```bash 
git branch -d {branch-name} # delete branch 
git branch -D {branch-name} # delete branch 
git branch -h # List more help
```

```bash 
# clean up local branches that are already merged AND also removed on the remote
git checkout main # main is your default branch. Change it to match your branch
git pull

git fetch --prune

git branch --merged | grep -v "\*" | grep -v "main" | xargs git branch -d
```

## Extra useful 

### Git stash 

```bash 
git stash -p -m "{your commit here}" # Stash to include message 
git stash -u # Include unstracked 
git stash -h # List more stash 
```

## TODO
- https://keep.google.com/u/0/#NOTE/1QkxJ35_8hle-FZB7ugJzCk-VGuSh14APK_x999FT_V4OtU_6i_T3Fn1151FZUaQ
