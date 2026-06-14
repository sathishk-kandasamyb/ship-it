# Lesson 2 — Saving Your Work Online

## Why this matters

Everything you committed in Lesson 1 lived only on your laptop.
If your laptop dies — your work is gone.

GitHub is your backup. Your safety net. Your online home for code.
`git push` sends your work there.

## Two places your code lives

```
your laptop          GitHub (online)
└── .git/        →   └── your repo
    commits           same commits
    history           same history
```

`commit` = save a snapshot on your laptop.
`push` = send that snapshot to GitHub.

## Connecting to GitHub — once only

Before you can push, you need to tell Git where to send your work.

```bash
git remote add origin https://github.com/yourusername/ship-it.git
```

`origin` is just a nickname for your GitHub repo.
You only do this once per project.

## Pushing for the first time

```bash
git push -u origin main
```

`-u` means "remember this connection forever."
After this, every future push is just:

```bash
git push
```

That's it. Git already knows where to send it.

## What the output means

```
Enumerating objects: 8, done.       ← Git counted everything
Writing objects: 100%               ← everything uploaded
new branch: main -> main            ← GitHub created main branch
branch 'main' set up to track       ← laptop and GitHub connected
```

No errors = it worked.

## Now break it on purpose

Disconnect your internet. Then try:

```bash
git push
```

You'll see a connection error.

> Git can commit without internet.
> Git can only push WITH internet.

Reconnect and push again. It works.

## Takeaway

> `commit` saves locally.
> `push` saves it to the world.
> Do both. Always.