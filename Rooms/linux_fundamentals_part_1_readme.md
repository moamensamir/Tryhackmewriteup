# Linux Fundamentals — Part 1

A beginner-friendly guide and walkthrough for the **LinuxFundamentalsPart1** room (TryHackMe style). This README is formatted for GitHub so you can copy it into a `README.md` file and share with others.

---

## Overview

This room is a basic, hands-on introduction to Linux for people starting their first career in cybersecurity or system administration. The exercises cover basic Linux concepts, navigation, file contents, simple commands, and searching for flags.

**Target audience:** beginners.

**Prerequisites:**
- A deployed Linux machine (or a TryHackMe lab machine)
- Basic familiarity with a terminal

---

## Task 1

Join the room to start. No command needed.

---

## Task 2

**Research:** What year was the first release of a Linux operating system?

**Answer:** `1991`

---

## Task 3

Open the machine using the room's web-based machine (SSH is optional — you can connect via the room machine).

---

## Task 4

Print `TryHackMe` in the terminal:

```bash
echo TryHackMe
```

Show the current username:

```bash
whoami
# Expected: tryhackme
```

---

## Task 5

**How many folders are on the machine?**

```bash
ls
# Example: 4
```

**Which directory contains a file?**

You can check each folder or use `du` to see sizes:

```bash
du
# One folder may be 8KB while others are 4KB — the larger one likely contains a file (e.g., folder4)
```

**What is the file content?**

```bash
cat note.txt
# Hello World
```

**What is the current path after navigating to the file?**

```bash
pwd
# /home/tryhackme/folder4
```

---

## Task 6

Use `grep` on `access.log` to find the flag that starts with `THM`.

```bash
cd /home/tryhackme
grep 'THM' access.log
# THM{ACCESS}
```

**Answer:** `THM{ACCESS}`

---

## Task 7

Run a command in the background:

```bash
# use &
command &
```

Replace the contents of `passwords` with `password123`:

```bash
echo password123 > passwords
```

Append `tryhackme` to the file while keeping existing content:

```bash
echo tryhackme >> passwords
```

---

That's the room solved step by step in a simple style for beginners.

