# Git and GitHub cheat sheet

Commands below apply to Git in a terminal. Replace placeholders with your own paths and names.

## Start and clone

```sh
git init
git clone https://github.com/OWNER/REPOSITORY.git
git status
```

## Stage and commit

```sh
git add README.md
git add .
git diff --staged
git commit -m "Describe the change"
```

Review `git status` and `git diff --staged` before committing. Never stage secrets or generated files accidentally.

## Branch and merge

```sh
git switch -c docs/update-guide
git switch main
git merge docs/update-guide
```

Resolve conflict markers in the affected files, test the result, then stage and commit the resolution.

## Push and pull

```sh
git remote -v
git push -u origin main
git pull --rebase
```

`origin` and `main` are common names, not guaranteed. Check the configured remote and branch first. A pull request is created on the hosting service after a branch is pushed; review changes before merging.

## Common errors

| Message or symptom | First checks |
| --- | --- |
| `rejected` / non-fast-forward | Fetch remote changes, inspect the history, then integrate intentionally. |
| `fatal: not a git repository` | Check the current folder and locate its `.git` directory. |
| Authentication failed | Confirm the remote URL and use the hosting provider's supported authentication method. Never put tokens in a URL or commit. |
| Merge conflict | Open each conflicted file, resolve markers, run checks, then stage the resolution. |

## `.gitignore` basics

Add project-specific generated files, local environments, caches, and secrets to `.gitignore` before staging. Ignore rules do not untrack a file already committed; remove it from the index carefully and rotate any exposed credential.

Further reading: [Pro Git](https://git-scm.com/book/en/v2) and [GitHub Docs](https://docs.github.com/en).
