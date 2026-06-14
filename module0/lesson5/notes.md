# Lesson 5 — Setting Up VS Code

## Why this matters

You can write code in any text editor.
But VS Code makes everything easier.
It shows your files, your Git changes, and your terminal — all in one place.

## What is VS Code?

VS Code is a free code editor made by Microsoft.
It works on Mac, Windows, and Linux.
It is the most popular code editor in the world.

## Install VS Code

Go to:
```
https://code.visualstudio.com
```

Click Download. Run the installer. Done.

---

## Open VS Code in your project folder

The best way to open VS Code is from the terminal.
Navigate to your project folder first:

```bash
cd ship-it
```

Then type:

```bash
code .
```

The `.` means "open this folder right here."
VS Code opens with your project loaded.

## Check it worked

```bash
code --version
```

You should see a version number like:
```
1.21.0
```

## The VS Code layout

```
LEFT SIDEBAR    — your files and folders
MAIN AREA       — where you write code
BOTTOM PANEL    — your terminal lives here
TOP RIGHT       — Source Control (Git)
```

## Open the terminal inside VS Code

You don't need to switch between VS Code and your terminal.
VS Code has a terminal built in.

**Mac:** press `Ctrl + `` ` ``
**Windows:** press `Ctrl + `` ` ``
**Linux:** press `Ctrl + `` ` ``

Same shortcut on all platforms.

A terminal opens at the bottom. 
This is your VS Code Integrated Terminal.
Everything you typed in your terminal — works here too.

## Open Source Control

Click the branch icon on the left sidebar.
Or press:

**Mac:** `Cmd + Shift + G`
**Windows/Linux:** `Ctrl + Shift + G`

You'll see your Git changes here.
Files you changed. Files you staged. All visual.

## Break it on purpose

Close VS Code.
Go to a folder that is NOT a Git repo:

```bash
mkdir not-a-repo
cd not-a-repo
code .
```

Open Source Control in VS Code.
You'll see:

```
No source control providers registered.
```

VS Code knows this folder has no Git.
It won't show Git features until you run `git init`.

## Takeaway

> VS Code is not just a text editor.
> It is your Git dashboard, your terminal, and your workspace — all in one.