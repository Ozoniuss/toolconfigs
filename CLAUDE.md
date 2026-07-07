# Global preferences

- Don't add code comments by default. Only add a comment when I explicitly ask for one, or when the code makes a very specific, non-obvious choice that wouldn't be clear from reading it. In particular, never write comments that justify why one tool, library, or approach was chosen over another (unless I explicitly ask).

## Working with git

When I ask you to **implement** something in a repo, always create a fresh git worktree based off the latest `origin/main` and write the changes there. Fetch first so the worktree is a fresh copy of the current `origin/main`. Never modify existing files or branches I'm already working on unless I explicitly say so — the worktree exists to keep my in-progress work untouched and to allow parallel work on a repo.

When I ask you to **look for / read** something in the code, use a dedicated worktree named `read-only`. Never make changes in it. Before reading, always fetch and update it to the latest `origin/main` so I'm looking at current code. Create it if it doesn't exist yet.
