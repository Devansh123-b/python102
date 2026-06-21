# Week 2 Exercises

Do these on your own, in your `week2-git-practice` repo. Each task ends with a push — that's how your instructor will check your work, by looking at your GitHub repo, not by checking your laptop.

Use the terminal for all of these. No GitHub Desktop, no VS Code Source Control panel — see `02_setup_and_clone.md` if you forgot why.

## Exercise 1: Your first independent file

Create a file called `about_me.py` that prints three lines: your name, your favorite Python101 project, and one thing you want to build by the end of Python102.

```python
print("Name: ...")
print("Favorite Python101 project: ...")
print("Goal for this course: ...")
```

Run the full cycle:

```bash
git add about_me.py
git commit -m "Add about_me.py"
git push
```

Confirm it shows up on your GitHub repo page.

## Exercise 2: Edit and re-commit

Open `about_me.py` again and add a fourth `print()` line: one thing you learned in Week 1 (VS Code, Python setup, etc.).

Commit and push this change **as a separate commit** — don't just edit and push without committing first.

```bash
git add about_me.py
git commit -m "Add Week 1 takeaway to about_me.py"
git push
```

When you're done, run `git log` and confirm you can see **two separate commits** for this file, each with its own message.

## Exercise 3: A second file, same repo

A repo can hold more than one file. Create `times_table.py`:

```python
number = 7
for i in range(1, 11):
    print(number, "x", i, "=", number * i)
```

Stage, commit, and push it — same cycle, new filename.

## Exercise 4: Write your own commit message

Make one more change of your choice — anything you've learned in Python101 or Python102 so far (a small function, a loop, a calculation). Save it as `extra.py`.

Before committing, write down what you think a **good** commit message would be, and what a **bad** one would look like, for this specific change. Use your good one.

```bash
git add extra.py
git commit -m "your message here"
git push
```

## Exercise 5: Read your own history

Run:

```bash
git log
```

Answer these for yourself (no need to write it down, just be ready to explain it if asked):

- How many commits do you have in total?
- Can you tell, just from the messages, what each commit did without re-reading the code?
- If a message doesn't make that clear, that's a sign it needs to be more specific next time.

## Done?

Check your repo on GitHub.com. You should see:

- [ ] `about_me.py` (edited at least once, so at least 2 commits touch this file)
- [ ] `times_table.py`
- [ ] `extra.py`
- [ ] At least 4 commits total, each with a message that actually describes the change

This repo and this workflow are the foundation for the rest of the course — every project from Week 3 onward gets added, committed, and pushed the same way.
