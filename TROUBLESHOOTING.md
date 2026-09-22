# C++ Troubleshooting Guide

If your C++ program does not compile or does not produce the expected output, use **GitHub Issues**.

The purpose is not only to fix the code. The purpose is to practice a real debugging workflow.

## Before Creating an Issue

Please do these first:

- Save your latest code.
- Compile again.
- Read the complete terminal error.
- Check the filename.
- Check missing semicolons.
- Check brackets `{}`.
- Check variable names.
- Try at least **one solution yourself**.
- Push the latest version to GitHub.

## How to Create an Issue

Open your own repository:

```text
Repository
→ Issues
→ New Issue
→ C++ Troubleshooting
```

Use a clear title:

```text
[HELP] linked_list.cpp cannot compile
```

Avoid titles such as:

```text
help
error
not working
sir please check
```

## Required Information

Your issue should include:

### Student

```text
Name:
NIM:
Class:
```

### Problem

Explain what you are trying to do.

### File

Example:

```text
linked_list.cpp
```

### Command

Example:

```powershell
g++ linked_list.cpp -o linked_list
.\linked_list.exe
```

### Error Message

Copy the **complete terminal error** into a code block.

### Expected Result

What did you expect your program to do?

### What I Already Tried

Write at least one attempt:

```text
1. Checked missing semicolon
2. Checked variable names
3. Recompiled the program
```

### Screenshot

Optional. A screenshot can help, but **text error messages are still required**.

## Mention the Instructor

At the bottom of your issue:

```text
@shiddiqeuy could you please help me troubleshoot this?
```

## After You Find the Solution

Do not leave the issue unfinished.

1. Fix the code.
2. Commit the solution.
3. Push it to GitHub.
4. Comment on the issue with the solution.
5. Close the issue.

Example:

```text
Solved.

Cause:
I forgot to initialize L.first to nullptr.

Fix:
Added createList(L) before inserting nodes.

Commit:
abc123
```

## Debugging Mindset

```text
Error
  ↓
Read
  ↓
Understand
  ↓
Make a hypothesis
  ↓
Change one thing
  ↓
Compile again
  ↓
Observe
  ↓
Repeat
```

The goal is to become better at **thinking through problems**, not only making the compiler error disappear.
