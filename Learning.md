# Learning Memo

## Create Branch
### ブランチ作成
```
git branch feature/01_create_branch
git branch feature/02_commit feature/01_create_branch
```

### ブランチ切り替え
```
git checkout feature/01_create_branch
```

***
## Commit & Push
### ファイル追加
```
git add Learning.md
```

### Commit
```
git commit -m "[Add] Learning.md"
```

### Push
```
git push origin feature/01_create_branch
```

***
## Pull Request
### Checkout PR
```
git fetch origin pull/1/head:pull_requests/pr-01
```

### Resolve conflicts
- Step 1: Clone the repository or update your local repository with the latest changes.  
※該当ブランチで実施すること
```
git pull origin main
```
- Step 2: Switch to the head branch of the pull request with the conflicts.
```
git checkout feature/02_commit
```

- Step 3: Merge the base branch into the head branch.
```
git merge main
```

- Step 4: Push the changes.
```
git push -u origin feature/02_commit
```

### iPhone GitHub Appの操作を試してみる。

- Step 1: Create Branch
```
git switch -c feature/04_pull_request_for_app
```
- Step 2: Commit & Push
- Step 3: Create PR  
  [git_learning/pull/4](https://github.com/long-910/git_learning/pull/4)


