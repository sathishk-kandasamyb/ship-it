# Lesson 6 — Setting Up Claude Code

## Why this matters

Claude Code is an AI assistant that lives in your terminal.
It can help you write code, fix errors, and understand Git.
It is not here to do your work for you.
It is here to help you think.

## What is Claude Code?

Claude Code is a command line tool made by Anthropic.
You talk to it by typing. It replies in your terminal.
It can see your files, your Git history, your errors.

Think of it as a senior developer sitting next to you.
You ask questions. It explains. You still do the work.

## Install Claude Code

Make sure you have Node.js installed first:

```bash
node --version
```

If you see a version number — you're ready.
If not — go to https://nodejs.org and install it first.

Then install Claude Code:

```bash
npm install -g @anthropic/claude-code
```

Check it worked:

```bash
claude --version
```

You should see a version number.

## Start Claude Code

Navigate to your project folder:

```bash
cd ship-it
```

Then start Claude Code:

```bash
claude
```

You'll see a prompt. Claude is ready.

## The fourth way to commit

You already know three ways to commit:
1. Terminal
2. VS Code Source Control
3. VS Code Integrated Terminal

Claude Code is the fourth way.

Inside Claude Code terminal you can run any Git command:

```bash
git add .
git commit -m "your message"
git push
```

Same commands. Same result. But now you have AI help right next to you.

## How to use Claude Code the right way

❌ Wrong:
```
"Write my commit message for me"
"Fix all my Git errors"
"Do the push for me"
```

✅ Right:
```
"I got this error, what does it mean?"
"Is my commit message clear enough?"
"Why did my push get rejected?"
```

Claude Code is a thinking partner. Not an autopilot.

## Break it on purpose

Inside Claude Code terminal type:

```bash
git stauts
```

See the typo error.
Now ask Claude:

```
"I got this error: git stauts — what did I do wrong?"
```

Claude will explain. You will fix it. You will learn it.

## Takeaway

> Claude Code doesn't replace learning Git.
> It makes learning Git faster and less frustrating.
> You still type every command. You still make every decision.