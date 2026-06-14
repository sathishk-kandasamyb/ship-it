# Lesson 4 — Your First Repo From Scratch

## The problem

You know the commands now.
But commands without order are just words.

The order matters.
Every single time.

Miss one step — Git gets confused.
Skip one step — your push fails.
Do them out of order — nothing works.

This lesson is about the order.

## The full loop — memorize this

```
1. mkdir project-name    — create the folder
2. cd project-name       — go inside it
3. git init              — give it a brain
4. create a file         — give Git something to watch
5. git add filename      — stage it
6. git commit -m "msg"   — snapshot it
7. git remote add origin url  — connect to GitHub
8. git push -u origin main    — send it online
```

Eight steps. Same order. Every time.

## Why this order?

You cannot stage before you have a file.
You cannot commit before you stage.
You cannot push before you commit.
You cannot connect to GitHub after you push.

Each step unlocks the next.
Like levels in a game.

## Try it yourself

Create a brand new project right now.
Not ship-it. A new one.

```bash
mkdir my-first-repo
cd my-first-repo
git init
```

Create a file:

```bash
echo "# My First Repo" > README.md
```

Check Git sees it:

```bash
git status
```

Stage it:

```bash
git add README.md
```

Commit it:

```bash
git commit -m "first commit"
```

Check your history:

```bash
git log --oneline
```

You did it. One snapshot. One commit. Your first repo.

## Now connect to GitHub

Go to github.com.
Create a new repository called `my-first-repo`.
Do NOT add a README — you already have one.

Copy the remote URL. Then run:

```bash
git remote add origin https://github.com/yourusername/my-first-repo.git
git push -u origin main
```

Go to GitHub. Refresh the page.
Your repo is live.

## Break it on purpose

Try pushing without connecting to GitHub first:

```bash
mkdir broken-repo
cd broken-repo
git init
echo "# test" > README.md
git add README.md
git commit -m "test"
git push
```

You'll see:
```
fatal: No configured push destination.
```

Git doesn't know where to send it.
You forgot step 7 — `git remote add`.

The order saved you. Now you know why it exists.

## The one thing beginners always forget

After `git init` — Git is watching.
But it is watching an empty room.

You must create a file.
You must stage it.
You must commit it.

THEN you can push.

Empty repos cannot be pushed.

## Takeaway

> Git is not magic. It is a sequence.
> Learn the order. Trust the order.
> Eight steps. Same every time.