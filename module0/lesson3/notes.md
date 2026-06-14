# Lesson 3 — Installing Git

## Why this matters

Lesson 1 showed you how to check if Git is installed.
If you saw `command not found` — this lesson is for you.

## Pick your operating system

---

### Mac

Mac sometimes has Git already.
Check first:

```bash
git --version
```

If you see a version number — skip this lesson. You're done.

If not — the easiest way is to install Xcode Command Line Tools:

```bash
xcode-select --install
```

A popup will appear. Click Install. Wait. Done.

Check again:

```bash
git --version
```

You should see a version number now.

---

### Windows

1. Go to https://git-scm.com/download/win
2. Download the installer
3. Run it — click Next on everything
4. When you see "Adjusting your PATH" — choose "Git from the command line and also from 3rd-party software"
5. Finish the install

Open Command Prompt or PowerShell and check:

```bash
git --version
```

You should see a version number.

---

### Linux

On Ubuntu or Debian:

```bash
sudo apt update
sudo apt install git
```

On Fedora:

```bash
sudo dnf install git
```

Check:

```bash
git --version
```

---

## After installing — one time setup

Tell Git who you are. Every commit will carry your name.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Check it worked:

```bash
git config --global user.name
git config --global user.email
```

You should see your name and email printed back.

## Break it on purpose

Try setting your name with a typo:

```bash
git config --global user.nme "Your Name"
```

Then check:

```bash
git config --global user.name
```

Nothing prints. Git saved the wrong key.
Fix it:

```bash
git config --global user.name "Your Name"
```

## Takeaway

> Git needs to know who you are before it can record your work.
> Set your name and email once. Git remembers forever.