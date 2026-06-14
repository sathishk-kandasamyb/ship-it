# Lesson 4 — Your First Terminal Commands

## Why this matters

Every Git command you run lives in the terminal.
If the terminal scares you — Git will scare you.
Let's fix that right now.

## What is the terminal?

It is a text window where you talk to your computer.
Instead of clicking — you type.
That's it.

```
you type a command → computer does it → shows you the result
```

## How to open it

**Mac** — press `Cmd + Space`, type `Terminal`, hit Enter

**Windows** — press `Windows key`, type `PowerShell`, hit Enter

**Linux** — press `Ctrl + Alt + T`

## The commands you need to know

### Where am I?

```bash
pwd
```

Stands for Print Working Directory.
Shows you which folder you are in right now.

Example output:
```
/Users/yourname/Documents
```

---

### What's in this folder?

```bash
ls
```

Lists everything in your current folder.

On Windows use:
```bash
dir
```

---

### Go into a folder

```bash
cd folder-name
```

`cd` stands for Change Directory.
Think of it like double clicking a folder.

Example:
```bash
cd ship-it
```

---

### Go back one folder

```bash
cd ..
```

`..` means "one folder up".
Like clicking the back button.

---

### Create a new folder

```bash
mkdir folder-name
```

`mkdir` stands for Make Directory.

Example:
```bash
mkdir my-project
```

---

### Create a new file

**Mac/Linux:**
```bash
touch filename.md
```

**Windows:**
```bash
echo. > filename.md
```

---

### Clear the screen

```bash
clear
```

Too much text? This cleans it up.
Your history is not deleted. Just hidden.

---

## Try it yourself

Do this right now in your terminal:

```bash
pwd
```

```bash
ls
```

```bash
mkdir practice-folder
```

```bash
cd practice-folder
```

```bash
pwd
```

See how you moved into the new folder?

## Break it on purpose

Try going into a folder that doesn't exist:

```bash
cd fake-folder
```

You'll see:
```
cd: fake-folder: No such file or directory
```

The terminal is not angry. It's just honest.
If something doesn't exist — it tells you.

## Takeaway

> The terminal is just a text version of your file explorer.
> Same folders. Same files. Just typed instead of clicked.