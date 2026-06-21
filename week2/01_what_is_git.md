# What is Git? What is GitHub?

## The problem they solve

You've probably had one of these happen:

- You changed something in a file and now you wish you hadn't, but there's no way back to the old version.
- You and a friend both edited the same document and one of you overwrote the other's work.
- Your laptop crashed and you lost a project.

Version control exists to fix all three of these.

## Two different tools, two different jobs

**Git** is a program that runs on your computer. It tracks changes to your project over time by saving snapshots. Every time you tell it to, Git records exactly what your files looked like at that moment. You can look back at any snapshot, compare snapshots, or go back to an older one.

**GitHub** is a website. It stores a copy of your Git project online. When you "push" your snapshots to GitHub, you're uploading your project's history so it's backed up and so other people can see it (or work on it with you).

A simple way to keep them separate:

> Git = the tool that tracks your changes. GitHub = the website that stores your tracked project online.

You will use both, every class, for the rest of this course.

## Why developers use this (not just students)

1. **Backup.** If your laptop dies, your code doesn't. It's already on GitHub.
2. **History.** You can see exactly what changed, when, and why — and undo any specific change without losing everything else.
3. **Collaboration.** Two people can work on the same project at the same time without overwriting each other's work.

This isn't a beginner tool that gets replaced with something more "professional" later. Software engineers at every company — from two-person startups to Google — use Git and GitHub exactly the way you're about to learn it.

## Where you've already seen this

Every file you've used in Python101 and Python102 so far came from a GitHub repository: `mathandcodingacademy/python102`. Someone (your instructor) used Git to create those files, took snapshots of them, and pushed them to GitHub — which is how they ended up on your screen.

Starting this week, you do that part yourself.

## A repository, defined

A **repository** (or "repo") is just a project folder that Git is tracking. It can live in two places at once:

- **Locally** — on your own computer, where you actually write and edit code.
- **Remotely** — on GitHub, where it's backed up and viewable online.

The next file (`02_setup_and_clone.md`) walks you through creating one of each, and connecting them.
