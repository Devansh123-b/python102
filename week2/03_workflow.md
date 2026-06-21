# The Core Workflow: add, commit, push

This is the one thing you will do every single class from now on. Once this feels automatic, the rest of the course is easy.

> **Make a change → `git add` it → `git commit` it → `git push` it.**

## What each command actually does

| Command | Job |
|---|---|
| `git add <file>` | Stage the file — tell Git "include this in my next snapshot" |
| `git commit -m "message"` | Take the snapshot, with a short note about what changed |
| `git push` | Upload your snapshots to GitHub |

You always do them in this order. You can `add` and `commit` as many times as you want before you `push` — pushing just uploads whatever commits you've built up so far.

## Round 1: do this step by step

Make sure you're inside your `week2-git-practice` folder in the VS Code terminal (`cd week2-git-practice` if you're not).

**1. Create a new file** called `hello.py` with this content:

```python
print("Hello, Git!")
```

**2. Check what Git sees:**

```bash
git status
```

`hello.py` will show up as **untracked** (usually in red). Git knows the file exists but isn't tracking it yet.

**3. Stage it:**

```bash
git add hello.py
```

Run `git status` again. Now `hello.py` shows as staged (usually in green) — it's ready to be committed.

**4. Commit it:**

```bash
git commit -m "Add hello.py"
```

The `-m` flag lets you attach a message in the same line. Every commit needs one. A good message says *what changed*, in a few words — `"Add hello.py"` is fine. `"stuff"` or `"asdf"` is not, because it tells you nothing six months from now when you're trying to find when a bug appeared.

**5. Push it:**

```bash
git push
```

Go to your repo page on GitHub.com and refresh it. `hello.py` is now there.

## Round 2: do this on your own

Now repeat the cycle without the hand-holding:

1. Open `hello.py` and add a second `print()` line.
2. Run `git status`, `git add`, `git commit -m "..."`, `git push` — in that order.
3. Refresh GitHub and confirm your change shows up.

If you get stuck, check the troubleshooting table below before asking for help — most issues here have a one-line fix.

## Seeing your history

Once you've made a couple of commits, you can see them with:

```bash
git log
```

This shows every snapshot you've taken, in order, with its message, author, and date. Press `q` to exit this view.

## Troubleshooting

| Symptom | Fix |
|---|---|
| `git: command not found` | Git isn't installed — install from [git-scm.com](https://git-scm.com), then restart VS Code |
| `fatal: not a git repository` | You're not inside the cloned folder — run `cd week2-git-practice` |
| A strange editor (Vim) opens after `git commit` | You forgot `-m "message"` — press `Esc`, type `:q!`, press Enter to exit without saving, then redo the commit with `-m` |
| `git push` keeps asking for login | A browser window should pop up to sign in — use that instead of typing a password directly |
| `git status` shows your file in red again after you already staged it | You edited the file after staging — run `git add` again to re-stage the new changes |
| `git push` fails with a message about "rejected" or "behind" | Ask your instructor — this means the GitHub copy has changes your local copy doesn't, which we'll cover in a later week |

## Checkpoint

Before moving to `04_exercises.md`, confirm:

- [ ] You've completed the full `add → commit → push` cycle at least twice
- [ ] Both commits are visible on your repo's GitHub page
- [ ] You can explain, in your own words, what each of the three commands does
