# Lesson 1 — What is Git and Why Does it Exist?

## Why this matters

You will use Git every single day as a developer.
Not because someone told you to.
Because without it — you will lose your work.

## The problem Git solves

Imagine this. You are writing code. It works.
You change something. Now it is broken.
You try to undo. You can't remember what you changed.

Or this. You and a teammate edit the same file.
You save yours. They save theirs.
One of you just deleted the other's work.

Git solves both of these problems.

## What is Git?

Git is a version control system.
It tracks every change you make to your files.
It remembers every version. Forever.

Think of it like a time machine for your code.
You decide when to save a snapshot.
You can go back to any snapshot. Anytime.

## Who created Git?

Linus Torvalds created Git in 2005.
He also created Linux.
He needed thousands of developers to work on the same code safely.
So he built Git in 10 days.

## How Git thinks

Git doesn't just save files.
It saves snapshots of your entire project.

```
snapshot 1 — just README.md
snapshot 2 — README + lesson1
snapshot 3 — README + lesson1 + lesson2
```

Every commit = one snapshot.
Every snapshot = your entire project at that moment.

## Git vs GitHub

These are not the same thing.

```
Git      — the tool on your laptop
           tracks changes, saves snapshots

GitHub   — a website
           stores your Git history online
           lets teams collaborate
```

You can use Git without GitHub.
But GitHub needs Git.

## Break it on purpose

Go to a folder with no Git:

```bash
mkdir no-git-here
cd no-git-here
git status
```

You'll see:
```
fatal: not a git repository
```

Git is not watching this folder.
It only watches folders where you ran `git init`.

Go back to ship-it:

```bash
cd ..
cd ship-it
git status
```

Now Git responds normally.

## Takeaway

> Git is not a backup tool. It is a time machine.
> You control when snapshots are taken.
> Every snapshot is permanent. Nothing is ever truly lost.