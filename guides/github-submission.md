# GitHub Submission Guide

Each student should maintain their own GitHub repository.

## Recommended Repository Name

```text
cpp-data-structure-assignment
```

## Recommended Structure

```text
cpp-data-structure-assignment/
│
├── README.md
├── 01-adt/
│   └── adt.cpp
├── 02-singly-linked-list/
│   └── sll.cpp
└── evidence/
    ├── terminal-adt.png
    └── terminal-sll.png
```

## Basic Git Workflow

From the project folder:

```powershell
git init
git add .
git commit -m "Complete C++ data structure assignment"
```

Connect your GitHub repository:

```powershell
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

For future updates:

```powershell
git add .
git commit -m "Fix linked list traversal"
git push
```

## README Requirements

Your student repository README should contain:

```markdown
# C++ Data Structure Assignment

Name:
NIM:
Class:

## ADT
What I implemented:
What I learned:

## Singly Linked List
What I implemented:
What I learned:

## Compile
g++ filename.cpp -o program

## Run
.\program.exe

## Reflection
What was difficult?
How did I solve it?
```

## Troubleshooting

If you have an error:

- Push the latest code.
- Open a GitHub Issue.
- Paste the complete error.
- Describe what you already tried.
- Mention `@shiddiqeuy`.

Do not rely only on screenshots sent through WhatsApp.
