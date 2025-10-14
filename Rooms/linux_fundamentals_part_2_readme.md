# Linux Fundamentals — Part 2

A beginner-friendly walkthrough for the **LinuxFundamentalsPart2** room (TryHackMe style).

---

## Overview

This room continues the basics for beginners: reading man pages, creating and moving files, checking file types and ownership, switching users, and identifying common Linux directories.

**Connect to the machine:**
- You can use the room's web-based machine or connect via SSH.
- SSH example:

```bash
ssh new-user@<IP>
# password: new-user
```

---

## Task 1 & 2

Read the instructions and start the machine (web machine or SSH). No further commands required here.

---

## Task 3 — Explore `ls` manual

**Question:** Explore the manual page of the `ls` command.

**Answer:**

```bash
man ls
```

**What directional arrow key would we use to navigate down the manual page?**

Answer: The down arrow key.

**What flag would we use to display output in a "human-readable" way?**

Answer: `-h` (see `man ls` for `-h`)

---

## Task 4 — Files and types

**4.1 How would you create the file named `newnote`?**

```bash
touch newnote
```

**4.2 What is the file type of `unknown1` in `tryhackme`'s home directory?**

```bash
file unknown1
# Expected: ASCII text
```

**4.3 How would we move the file `myfile` to the directory `myfolder`?**

```bash
mv myfile myfolder
```

**4.4 What are the contents of this file (`myfile`)?**

```bash
cat myfile
# Expected: THM{FILESYSTEM}
```

---

## Task 5 — Ownership and switching users

**On the deployable machine, who is the owner of `important`?**

Use `ls -la` to view owner details — expected owner: `user2`.

**What is the command to switch to the user `user2`?**

```bash
su user2
# then enter the password for user2
```

**Output the contents of `important`. What is the flag?**

```bash
cat important
# Expected: THM{SU_USER2}
```

---

## Task 6 — Common directories

**What directory path would we expect logs to be stored in?**

Answer: `/var`

**What root directory is similar to how RAM on a computer works? (contents do not persist after reboot)**

Answer: `/tmp`

**Name the home directory of the root user**

Answer: `/root`

---

That's the Part 2 walkthrough. If you want this translated to Arabic, shortened, or formatted for a specific GitHub repo template, tell me and I'll update it.
