# AwesomeGitTips

### Git Large file storage 

> Install
```
git lfs install
```

> Track large file type
```
git lfs track "*.<file-type>"
```

> Add tracking file
```
git add .gitattributes
```
_Note:_ See more about [git lfs migrate](https://github.com/git-lfs/git-lfs/blob/main/docs/man/git-lfs-migrate.adoc?utm_source=gitlfs_site&utm_medium=doc_man_migrate_link&utm_campaign=gitlfs) when your file is still refused


### Git Submodule

> Go to target folder that you wanna add sub-repo

> Add submodule 
```
git submodule add --reference <./new-folder-name> <repo-link-to-clone>
```
> Remove submodule

```
git rm -rf <./new-folder-name>
```
```
git rm -rf <./.gitmodules>
```

### Compare commits of two git branches

```
git log branch1..branch2
```

### Combine multiple commits

> Step 1. 
```
git rebase -i head~n
```
- n: number of commits need to combine

> Step 2.

- Remain 1 commit and change `pick` to `squash` for the rest commits

- Save file (and commit if needed)

> Step 3.
```
git rebase --continue
```



## Ref:
1. [Khoi phuc code bang git reflog](https://tuanndl.com/post/khoi_phuc_code_bang_git_reflog)
2. [Refresh after update gitignore file](https://shrestharohit.com.np/file-added-to-gitignore-still-showing-in-untracked-list/)
3. [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
4. [Tái sử dụng code cho nhiều project với Git Submodules](https://techmaster.vn/posts/36659/tai-su-dung-code-cho-nhieu-project-voi-git-submodules#:~:text=Git%20Submodules%20cho%20ph%C3%A9p%20t%E1%BA%A1o,d%E1%BB%A5ng%20theo%20d%E1%BA%A1ng%20Sub%20module)
5. [Git lfs document](https://git-lfs.com/)
