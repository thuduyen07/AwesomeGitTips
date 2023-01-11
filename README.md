# AwesomeGitTips

### Compare commits of two git branches

```
git log branch1..branch2
```

### Combine multiple commits

> Step 1. 
```
git rebase -i head~n
```
n: number of commits need to combine

> Step 2.
Remain 1 commit and change `pick` to `squash` for the rest commits

Save file (and commit if needed)

> Step 3.
```
git rebase --continue
```


## Ref:
1. [Khoi phuc code bang git reflog](https://tuanndl.com/post/khoi_phuc_code_bang_git_reflog)
2. [Refresh after update gitignore file](https://shrestharohit.com.np/file-added-to-gitignore-still-showing-in-untracked-list/)
