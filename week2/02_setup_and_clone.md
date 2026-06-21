# Setting Up Git and Creating Your First Repo

## Step 1: Set your Git identity

Git attaches a name and email to every snapshot you save, so there's a record of who made each change. This is a one-time setup — you won't need to do it again.

Open the terminal in VS Code and run these two commands, replacing the example name and email with your own:

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

This isn't a login. Nobody checks this email is real, and it's not connected to your GitHub password. It's just a label that gets attached to your work.

## Step 2: Create a repository on GitHub.com

1. Go to [github.com](https://github.com) and make sure you're logged in.
2. Click the green **New** button (or the **+** icon in the top right → **New repository**).
3. Repository name: `week2-git-practice`
4. Keep visibility set to **Public**.
5. Check the box for **Add a README file**.
6. Click **Create repository**.

You now have a repository on GitHub's servers with one file in it (`README.md`). Nothing is on your laptop yet — that's the next step.

## Three ways to use Git — and which one we use in this course

You have **GitHub Desktop** installed, and you'll also see Git built into VS Code. There's also the terminal, which is what this course uses. All three do the exact same job — they just look different.

| Tool | What it is | Used in this course? |
|---|---|---|
| **Terminal (command line)** | Typing commands like `git add`, `git commit`, `git push` directly | **Yes — this is what we use** |
| **GitHub Desktop** | A separate app with buttons instead of commands | No, not in class — but fine for personal projects |
| **VS Code's built-in Git** | Buttons inside VS Code's Source Control panel | No, not in class — same reason as Desktop |

**Why the terminal, when buttons are easier?**

Buttons hide what's actually happening. When you click "Commit" in GitHub Desktop or VS Code, it runs the exact same `git commit` command you'll learn in `03_workflow.md` — you just don't see it. Typing the commands yourself means:

- You learn what each step is actually called, which matters when you're searching for help online — every tutorial, every error message, every Stack Overflow answer uses the command names, not button labels.
- You can tell the difference between Git itself and whichever app happens to be wrapping it.
- It's the same skill whether you're on this laptop, a different computer, or a server with no GUI at all.

**If you already use GitHub Desktop at home:** that's fine for your own projects. For this course, every exercise and every checkpoint expects you to use the terminal — partly so everyone in class is looking at the same screen, and partly because typing the commands is the whole point of this week's lesson.

## Step 3: Clone the repo to your computer

**Clone** means downloading a full copy of a GitHub repo onto your computer, including its entire history.

1. On your repo's GitHub page, click the green **Code** button.
2. Make sure **HTTPS** is selected, then copy the URL shown (it ends in `.git`).
3. In the VS Code terminal, navigate to the folder where you keep your course files, then run:

```bash
git clone https://github.com/YOUR-USERNAME/week2-git-practice.git
```

4. Move into the new folder:

```bash
cd week2-git-practice
```

5. Open this folder in VS Code (**File → Open Folder**, or run `code .` in the terminal) and confirm you can see `README.md`.

**Note:** once you open a cloned repo in VS Code, you'll notice a **Source Control** icon appear in the left sidebar (it looks like a branching line). That's VS Code's built-in Git panel from the table above. Ignore it for this course — we're typing every command ourselves in the terminal at the bottom of the screen, not clicking that panel.

## Checkpoint

Before moving to `03_workflow.md`, confirm:

- [ ] `git --version` works in your terminal without an error
- [ ] You ran the two `git config` commands with your own name and email
- [ ] You created `week2-git-practice` on GitHub.com
- [ ] You cloned it and can see the `README.md` file inside VS Code

If any of these aren't true yet, fix it now — everything in the next file depends on having a repo cloned locally.
