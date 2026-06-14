# Module 1 Challenge — Solution

## The three problems

### Problem 1 — Wrong order
`git add` was run before `cd my-project` and `git init`.
You cannot use Git commands outside a repo.

### Problem 2 — No file exists
`git add README.md` was run but README.md was never created.
You cannot stage a file that doesn't exist.

### Problem 3 — git init came too late
`git init` must always come first.
Before add. Before commit. Before everything.

## The correct order

```bash
mkdir my-project
cd my-project
git init
echo "# My Project" > README.md
git add README.md
git commit -m "first commit"
```

## Why this matters

Git is a sequence. Not a collection of commands.
Each step unlocks the next.
The order is not optional.

## Takeaway

> When Git breaks — read the error.
> The error always tells you which step went wrong.