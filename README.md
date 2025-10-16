Git Initialization, Staging, Committing, Merging, Resetting, and Tagging

1. Git Initialization

Git is a version control system that helps track changes in source code during development.
To start using Git in a project, the repository must first be initialized.

Command:

git init

This command creates a hidden folder .git/ in the project directory, which stores all version control information.


2. Staging Files

After creating or modifying files, they need to be added to the staging area before committing.

Command:

git add <filename>

To stage all files at once:

git add .

The staging area acts as a preview of what will be committed to the repository.


3. Committing Changes

Once files are staged, they can be permanently recorded in the Git history with a commit message.

Command:

git commit -m "Initial commit"

Each commit represents a checkpoint in the project’s development timeline.


4. Adding and Committing New or Changed Files

When new files are created or existing files are modified, they can be added and committed as follows:

git add <new_or_modified_file>
git commit -m "Added new feature or updated file"

This ensures all updates are version-tracked properly.


5. Merging Branches

When multiple branches are used for development, Git allows merging to combine changes from one branch into another.

Example:

git checkout main
git merge feature-branch

If conflicts occur, Git will prompt the user to resolve them manually before completing the merge.


6. Reset or Discard Changes

To undo changes or reset the working directory:

To unstage a file (keep changes but remove from staging):

git reset <file>

To discard local changes (revert to last commit):

git checkout -- <file>

To completely reset the branch to a previous commit:

git reset --hard <commit_id>


7. Tagging (Version 10.0)

Tags are used to mark specific points in history as important — often used for version releases.

Command:

git tag v10.0
