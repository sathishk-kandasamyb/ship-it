# Lesson 2 — What is a Repository?

## The problem

You have a folder on your laptop called `my-project`.
Inside it — some files. Some code. Some work.

Git does not care about that folder.
Git does not watch it.
Git does not remember anything about it.

It is just a folder.

Until you say otherwise.

## What changes everything

```bash
git init
```

One command. That is all.

The moment you run it — your ordinary folder becomes a repository.
Git starts watching. Git starts remembering.
Nothing looks different from the outside.
But everything has changed on the inside.

## What actually happened

Git created a hidden folder inside your project:

```
my-project/
└── .git/        ← this appeared
```

That `.git` folder is Git's brain.
Every snapshot you ever take lives in there.
Every commit message. Every change. Every version.

You never open it. You never edit it.
But it is always there. Quietly remembering everything.

## Try it yourself

```bash
mkdir my-project
cd my-project
ls -la
```

You see nothing special. Just an empty folder.

Now run:

```bash
git init
ls -la
```

See that `.git` folder that appeared?
That is the moment your folder became a repository.

## Two kinds of repository

Right now you have two copies of Ship It.

```
One on your laptop     — only you can see it
One on GitHub          — the whole world can see it
```

They are called:

```
local repo     — your laptop
remote repo    — GitHub
```

Every time you push — they sync.
Every time you pull — they sync.
They are always trying to be identical.

## Break it on purpose

Step outside your repo:

```bash
cd ..
git status
```

You will see:

```
fatal: not a git repository
```

Git is not angry. It is just telling you the truth.
This folder has no `.git` brain. So Git knows nothing about it.

Step back in:

```bash
cd my-project
git status
```

Git responds immediately.
Same you. Same terminal. Different folder. Completely different result.

That `.git` folder is the only difference.

## Takeaway

> `git init` doesn't change your files.
> It gives your folder a brain.
> That brain remembers everything. Forever.