# /ship

Commit staged (or all) changes and push to remote in one step.

## Usage

```
/ship           — commit staged changes
/ship -y        — commit staged changes, bypass main/master guard
/ship all       — stage everything and commit
/ship all -y    — stage everything and commit, bypass main/master guard
/ship dry       — preview staged diff and proposed commit message without committing
```

## Behavior

- Derives a commit message from the diff, matching the style of recent commits in `git log`
- Refuses to push directly to `main` or `master` unless `-y` is passed
- In `dry` mode, prints the diff summary and proposed message, then stops — nothing is committed or pushed
- `-y` bypasses the branch guard only; it does not force-push

## Notes

- To preview all changes in `dry` mode, stage them first: `git add -A`
- If the repository has no commits yet, falls back to standard imperative mood style
- Commit messages follow imperative mood ("Add feature", not "Added feature") with no AI attribution
