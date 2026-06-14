# Lesson 1 — Is Git installed?

## Why this matters

Before you use Git, your computer needs to have it.
Most computers don't come with it ready.
Let's check if yours does.

## What is git --version?

It's a question you ask Git.
"Hey, are you there?"

If Git is installed, it answers with its version number.
If not, you'll see an error.

## Try it yourself

Open your terminal and type:

```bash
git --version
```

You should see something like:

```
git version 2.50.1
```

That means Git is installed. You're ready.

## What if you see an error?

If you see:
```
command not found: git
```

Git is not installed. Go to lesson 2 — Installing Git.

## Now break it on purpose

Type this:

```bash
git --versoin
```

You'll see:
```
error: unknown switch `e'
```

Git doesn't autocorrect. Ever.
One typo = one error.
Spelling is exact. Always.

## Takeaway

> git --version doesn't just show a number.
> It proves Git exists on your machine.