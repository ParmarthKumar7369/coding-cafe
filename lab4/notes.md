# Lab 4: Git & GitHub — Answers

### Question 1
**What did `--global` mean here? What would happen if you left it out? Guess, then check with `man git-config` or ask.**

`--global` means the configuration applies to all Git repositories belonging to my current Linux user. If I leave it out, Git applies the setting to the current repository, provided I run the command inside a Git repository.

### Question 2
**What appeared in `ls -a` but not in `ls`? What is inside it?**

The `.git` directory appeared in `ls -a` but not in `ls` because its name starts with a dot, making it hidden by default. It contains Git's internal repository data, including commit history, configuration, references, and stored objects.

### Question 3
**Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did *not* write?**

Initially, Git offered to track my untracked lab files and folders, including the files under week02/. The .venv/ directory contained installed packages and other files I did not write myself, so it should be excluded using .gitignore.

### Question 4
**Compare this `git status` with the one from Question 3. What disappeared?**

After creating `.gitignore`, files inside `.venv/`, along with other matching files such as Python bytecode and cache files, no longer appeared as untracked items. Git now ignores files matching the rules listed in `.gitignore`.

### Question 5
**`.gitignore` itself shows up as untracked. Should it be committed, or ignored too? Why?**

`.gitignore` should be committed because it contains rules that tell Git which files and directories to ignore. Committing it allows everyone working on the repository to use the same ignore rules.

### Question 6
**`README.md` moved from one heading to another in the `git status` output. Which two? In the three-places model from the session, what just happened to it?**

`README.md` moved from the "Untracked files" or "Changes not staged for commit" section to the "Changes to be committed" section. Running `git add README.md` staged the file, moving its changes from the working directory into the staging area.

### Question 7
**What did Git print after the commit? How many files did it say changed?**

Git printed a summary showing the commit identifier, commit message, and the files changed. It reported that 3 files changed, with 177 insertions.

### Question 8
**What are the first seven characters of your commit called, and what are they for?**

The first seven characters are the short form of the commit hash, a unique identifier for that commit. They let me identify and refer to a specific commit without typing its entire hash.

### Question 9
**You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?**

The four steps are edit, stage, commit, and repeat. Editing changes files, staging selects the changes to include, and committing saves those staged changes as a snapshot in the repository's history.

### Question 10
**Why does this file get a special name and a special place, rather than being called `notes.md` like everything else?**

GitHub automatically displays `README.md` on the repository's front page and formats its Markdown for easy reading. It introduces the project and helps visitors understand what the repository contains.

### Question 11
**What did `gh auth login` do that means you will not be asked for a password when you push?**

`gh auth login` authenticated my GitHub account through the browser and saved authentication credentials on my computer. Git can use these credentials when communicating with GitHub, so I do not have to enter my account password every time I push.

### Question 12
**Refresh the repository page on GitHub. What is showing on the front page, and why that file?**

The contents of `README.md` are displayed on the repository's front page. GitHub automatically renders this specially named file as formatted Markdown to introduce the repository and its contents.

### Question 13
**Run `git log --oneline` again. Did pushing change your local history in any way?**

No, pushing did not change my local commit history. It uploaded my existing commits to GitHub, creating a remote copy of the history.

### Question 14
**Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?**

A private repository exists on GitHub, but only its owner and people who have been granted access can view it. If a repository does not exist on GitHub, there is no remote repository there for people to access.
