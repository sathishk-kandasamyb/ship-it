Create this file:

```
ship-it/
└── module1/
    └── lesson3/
        └── notes.md
```

Then type this inside it:

````markdown
# Lesson 3 — What is a Commit?

## The problem

You have been saving your files.
Ctrl+S. Over and over.

But saving a file and committing are not the same thing.

When you save — your old version is gone.
Replaced. Overwritten. Forever.

When you commit — nothing is lost.
Every version lives. Side by side. Forever.

## What is a commit?

A commit is a snapshot.

Not just of one file.
Of your entire project. At one moment in time.

```
commit 1 — your project at 10:00am
commit 2 — your project at 10:30am
commit 3 — your project at 11:00am
```

You can go back to any of these moments.
Anytime. In seconds.

## What a commit remembers

Every commit stores three things:

```
WHAT   — exactly what changed
WHO    — who made the change (your name and email)
WHEN   — the exact date and time
WHY    — your commit message
```

That last one — the WHY — is the only one you write yourself.
Make it count.

## What makes a good commit message?

Bad:
```
git commit -m "stuff"
git commit -m "fixed it"
git commit -m "changes"
```

Good:
```
git commit -m "module1/lesson3: add what is a commit lesson"
git commit -m "fix: correct typo in README"
git commit -m "module0: update VS Code install instructions for Windows"
```

Good messages tell a story.
Three months from now — you will thank yourself.

## The staging area

Before you commit — you stage.

Think of it like packing a box before shipping.

```
your files          staging area        committed
(untracked)   →    (packed box)    →   (shipped)
git add             git commit
```

You choose what goes in the box.
You seal it when you're ready.
Git ships it.

## Try it yourself

Make a small change to any file.
Then check what Git sees:

```bash
git status
```

Stage it:

```bash
git add filename
```

Check again:

```bash
git status
```

See how it moved from untracked to staged?
Now commit it:

```bash
git commit -m "your message here"
```

## Break it on purpose

Try committing without staging anything:

```bash
git commit -m "nothing staged"
```

You'll see:
```
nothing to commit, working tree clean
```

Git won't commit thin air.
You must stage first. Always.

## Takeaway

> Saving a file = replacing the old version.
> Committing = adding a new snapshot. Nothing is lost.
> Every commit is a moment in time you can return to.
````

Save the file. Then come back. 🚢