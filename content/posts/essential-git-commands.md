---
date: 2025-01-05
title: "Git commands I use daily: From terminal fear to confident workflows"
---

In my previous role as a solo tech writer for a fintech company, we worked entirely in docs-as-code, documenting everything using code workflows from Visual Studio Code. As someone who used to fear the terminal, I made a choice to use only the terminal and become proficient in git commands, even if it meant breaking things.

And yes, I broke things. A lot.

Lucky for me, I had a developer who became my go-to lifeline: Javier. Every time I broke something (which was frequently), he'd patiently walk me through the fix. Those messy days and his patience taught me more than any tutorial ever could. I went from avoiding the command line to embracing it, mistakes and all. 

Here's my Git flow and the commands that became part of my daily workflow. The ones I learned through trial, error, and a very patient developer.

---

## My daily Git flow

### 1. Start every session with a status check

Before touching any code or documentation, I'd run:
```bash
$ git status  # using my alias for git status
```

This simple habit saved me countless times from working on the wrong branch or committing changes to the wrong place. It became my safety net.

### 2. Create feature branches for every change
```bash
$ git checkout -b feature/update-api-docs  # using alias for checkout
```

One feature, one branch. This kept my work organized and made it easier to switch tasks when priorities shifted.

### 3. Make small commits and keep them clean with amend

After my first commit:
```bash
$ git commit -m "Add new API documentation"  # using alias for commit
```

If I noticed something missing or wanted to adjust the same change, I didn’t create a new “fix” commit. Instead, I used ```git commit --amend```.
```bash
$ git add .
$ git commit --amend --no-edit
```

This kept my commit history clean from the start. No extra cleanup needed later.

### 4. Push to remote and open pull request
```bash
$ git push -u origin feature/update-api-docs
```

Then open a pull request (a request for someone to review my changes) for the team to review.

### 5. Use stash when switching tasks mid-work

Sometimes I’d be halfway through something and need to switch branches. Instead of committing half-baked changes, I stashed them:
```bash
$ git stash           # save current changes temporarily
$ git checkout other-branch # switch branches
$ git stash pop       # bring changes back later
```
Think of this as my “pause and come back later” button.

---

These six workflow steps became my daily rhythm. But they only worked because I understood the commands powering them. Here's what each command does and why it mattered to my workflow.

## The core commands that made it all work

### Creating aliases: Custom shortcuts

The aliases that changed everything, early on, I learned how to create Git aliases(shortcuts for longer commands). Following the [Git Basics - Git Aliases](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases) documentation, I set up:
```bash
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.st status
```

When you're breaking things daily, speed matters, but so does reducing typos. These shortcuts built my muscle memory and confidence.

But aliases are just shortcuts. To really understand my workflow, here are the actual commands I was running every day:

## The core commands I used daily:

- `git clone` – Create a local copy of a remote repository (the main project stored online)
- `git branch` – Create, list, and delete branches (separate workspaces for different features)
- `git checkout` – Switch between branches
- `git add` – Stage changes for commit (mark files ready to save)
- `git commit` – Save changes to the local repository (your computer's version)
- `git push` – Upload local commits to a remote repository (share with the team)
- `git status` – Check what's staged, unstaged, and which branch I'm on
- `git stash` / `git stash pop` – Temporarily save and retrieve work in progress
- `git checkout --` – Discard unstaged changes
- `git commit --amend --no-edit` – Update the last commit without changing the message

---

## Another tip from Javier: keeping commits clean

As I started committing more frequently, a pattern appeared. I’d make a commit… and then immediately realize:

- I’d missed a file
- there was a small typo
- there was one more change I meant to include

That’s when Javier introduced me to a simple but powerful command: `git commit --amend`

Instead of creating extra “fix” commits for tiny adjustments, I could update the previous commit and keep my history clean.

Why this worked so well for me

- it kept my commit history tidy and focused
- I didn’t have to learn more complex tools right away
- it helped me think in terms of complete changes, not fragments
- it removed one more thing to worry about before merging

When to use `--amend`

- you’re still working on the same logical change
- you haven’t pushed the commit to the remote yet
- you want to update or extend the most recent commit

This lesson from Javier became part of my workflow. Instead of making messy commits and cleaning them up later, I got into the habit of keeping my history clean from the start. It’s a small practice, but it made a big difference in how confidently I worked.


These commands and this workflow didn't come naturally. They came from breaking things, asking questions, and having someone patient enough to help me learn. 

From fearing the terminal to embracing it, the journey taught me that the messy part is where the real learning happens.


