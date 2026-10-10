# Lab 4: Git and GitHub

## Q1. What does --global mean?
The --global option applies Git configuration to all repositories associated with my Linux user account. This means I do not need to configure my name and email separately for each repository.

## Q2. What is the .git directory?
The .git directory stores Git's internal repository data, including commit history, configuration, references, and objects. Git uses this information to track changes and manage versions of the project.

## Q3. How many untracked folders were present?
Git initially showed one untracked folder, week02/. The .venv directory did not appear in the untracked list, indicating that it was already being ignored.

## Q4. What does .gitignore do?
The .gitignore file tells Git to ignore files matching specified patterns, such as Python virtual environments and cache files. These files do not appear as untracked files when they match the ignore rules.

## Q5. Why should .gitignore be committed?
Committing .gitignore shares the ignore rules with other people working on the repository. This helps prevent unnecessary files from being accidentally tracked.

## Q6. What is the difference between untracked and staged files?
Untracked files are not yet included in Git's tracking for a commit. Staged files have been selected using git add and are ready to be included in the next commit.

## Q7. How many files did the first commit change?
[Fill in the number shown by the git commit output.]

## Q8. What is the short SHA of the first commit?
The short SHA is a10af3d. A SHA is a unique identifier used by Git to identify a commit.
